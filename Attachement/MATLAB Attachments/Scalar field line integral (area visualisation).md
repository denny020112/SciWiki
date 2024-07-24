#MATLAB 
![[Scalar field line integral (area visualisation).png]]
```MATLAB
% 그래프 설정
figure;
hold on;
grid on;
view(3);

% 나선 경로 정의
t = linspace(0, 4*pi, 1000);
a = 0.5; % 나선의 간격을 조절하는 파라미터
r = a * t;
x = r .* cos(t);
y = r .* sin(t);

% 스칼라 함수 정의
f = @(x,y) 0.5 * (x.^2 + y.^2);

% 함수 값 계산
z = f(x, y);

% 경로를 따라 선적분 계산
ds = sqrt(diff(x).^2 + diff(y).^2);
integral_value = sum(f(x(1:end-1), y(1:end-1)) .* ds);

% 3D 곡선 그리기
plot3(x, y, z, 'b', 'LineWidth', 2);

% 장막 효과 만들기
surf([x; x], [y; y], [zeros(size(z)); z], 'FaceAlpha', 0.5, 'EdgeColor', 'none');

% 바닥에 등고선 그리기
[X, Y] = meshgrid(linspace(min(x), max(x), 50), linspace(min(y), max(y), 50));
Z = f(X, Y);
contour3(X, Y, zeros(size(Z)), Z, 20, 'k');

% 축 레이블 및 제목
xlabel('x');
ylabel('y');
zlabel('f(x,y)');
title(sprintf('Scalar field line integration visualisation\n integration val. = %.2f', integral_value));

% 컬러바 추가
colorbar;

% 범례 추가
legend('Integration Path(C)', 'Surface');
saveas(gcf,"Scalar field line integral (area visualisation).png")
```