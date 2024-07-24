#MATLAB 
![[vector field line integral.png]]
```MATLAB
% 그리드 생성
[x, y] = meshgrid(-2:0.2:2, -2:0.2:2);

% 벡터장 정의 (예: F(x,y) = [y, x])
u = y;
v = x;

% 적분 경로 정의 (원)
t = linspace(0, 2*pi, 100);
r = 1;
xc = r * cos(t);
yc = r * sin(t);

% 그림 생성
figure('Position', [100, 100, 600, 500]);

% 벡터장 그리기
quiver(x, y, u, v, 'b');
hold on;

% 적분 경로 그리기
plot(xc, yc, 'r', 'LineWidth', 2);

% 경로 상의 벡터 표시
s = 1:5:length(t);
quiver(xc(s), yc(s), u(round(yc(s)*5+11), round(xc(s)*5+11)), ...
    v(round(yc(s)*5+11), round(xc(s)*5+11)), 0.5, 'r', 'LineWidth', 1.5);

% 그래프 꾸미기
title('Line Integral of Vector Field');
xlabel('x');
ylabel('y');
axis equal tight;
grid on;
legend('Vector Field', 'Integration Path', 'Vectors along Path');

% 수식 추가
text(0, 2.5, '$\int_C \mathbf{F} \cdot d\mathbf{r} = \int_a^b \mathbf{F}(r(t)) \cdot \mathbf{r}''(t) dt$', ...
    'Interpreter', 'latex', 'FontSize', 14, 'HorizontalAlignment', 'center');

% 선적분 값 계산 (근사)
ds = sqrt(diff(xc).^2 + diff(yc).^2);
u_path = interp2(x, y, u, xc(1:end-1), yc(1:end-1));
v_path = interp2(x, y, v, xc(1:end-1), yc(1:end-1));
line_integral = sum((u_path .* diff(xc) + v_path .* diff(yc)));

% 선적분 값 표시
text(0, -2.5, sprintf('Approximate Line Integral Value: %.4f', line_integral), ...
    'FontSize', 12, 'HorizontalAlignment', 'center');
```