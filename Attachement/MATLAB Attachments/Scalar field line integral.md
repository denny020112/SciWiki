#MATLAB 
![[scalar field line integral 2D.png|500]]

![[scalar field line integral 3D.png|500]]
```MATLAB
% 그리드 생성
[x, y] = meshgrid(-2:0.1:2, -2:0.1:2);

% 스칼라장 정의 (예: f(x,y) = x^2 + y^2)
f = x.^2 + y.^2;

% 적분 경로 정의 (원)
t = linspace(0, 2*pi, 100);
r = 1;
xc = r * cos(t);
yc = r * sin(t);

% 그림 생성
figure('Position', [100, 100, 600, 500]);

% 스칼라장 등고선 그리기
contourf(x, y, f, 20, 'EdgeColor', 'none');
colorbar;
hold on;

% 적분 경로 그리기
plot(xc, yc, 'r', 'LineWidth', 2);

% 그래프 꾸미기
title('Line Integral of Scalar Field');
xlabel('x');
ylabel('y');
axis equal tight;
grid on;
legend('Scalar Field', 'Integration Path');

% 수식 추가
text(0, 2.5, '$\int_C f(x,y) ds = \int_a^b f(x(t),y(t)) \sqrt{(x''(t))^2 + (y''(t))^2} dt$', ...
    'Interpreter', 'latex', 'FontSize', 14, 'HorizontalAlignment', 'center');

% 선적분 값 계산 (근사)
ds = sqrt(diff(xc).^2 + diff(yc).^2);
f_path = interp2(x, y, f, xc(1:end-1), yc(1:end-1));
line_integral = sum(f_path .* ds);

% 선적분 값 표시
text(0, -2.5, sprintf('Approximate Line Integral Value: %.4f', line_integral), ...
    'FontSize', 12, 'HorizontalAlignment', 'center');

% 스칼라 값을 경로 위에 표시
s = 1:5:length(t);
scatter3(xc(s), yc(s), interp2(x, y, f, xc(s), yc(s)), 40, 'r', 'filled');

% 3D 표면 플롯 추가
figure('Position', [700, 100, 600, 500]);
surf(x, y, f, 'EdgeColor', 'none', 'FaceAlpha', 0.7);
hold on;
plot3(xc, yc, interp2(x, y, f, xc, yc), 'r', 'LineWidth', 2);
scatter3(xc(s), yc(s), interp2(x, y, f, xc(s), yc(s)), 40, 'r', 'filled');

title('3D View of Scalar Field Line Integral');
xlabel('x');
ylabel('y');
zlabel('f(x,y)');
colorbar;
grid on;
legend('Scalar Field', 'Integration Path');
```