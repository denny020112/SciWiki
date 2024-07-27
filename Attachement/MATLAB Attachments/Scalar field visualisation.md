#MATLAB 
![[scalar field visualisation.png]]
```MATLAB
% 그리드 생성
[x, y] = meshgrid(-3:0.1:3, -3:0.1:3);

% 스칼라장 정의 (예: f(x,y) = x^2 + y^2 - 2*x*y)
f = x.^2 + y.^2 - 2*x.*y;

% 그림 생성
figure('Position', [100, 100, 1000, 400]);

% 등고선 그래프
subplot(1, 2, 1);
contourf(x, y, f, 20);
colorbar;
title('Scalar Field - Contour Plot');
xlabel('x');
ylabel('y');
axis equal;

% 3D 표면 그래프
subplot(1, 2, 2);
surf(x, y, f);
colorbar;
title('Scalar Field - 3D Surface Plot');
xlabel('x');
ylabel('y');
zlabel('f(x,y)');
axis equal;

% 전체 그림 제목
sgtitle('Visualization of Scalar Field f(x,y) = x^2 + y^2 - 2xy', 'FontSize', 16);
```
