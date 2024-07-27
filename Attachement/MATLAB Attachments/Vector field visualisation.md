#MATLAB 
![[vector field visualisation.png]]
```MATLAB
% 그리드 생성
[x, y] = meshgrid(-2:0.2:2, -2:0.2:2);

% 벡터장 정의 (예: F(x,y) = [y, -x])
u = y;
v = -x;

% 그림 생성
figure('Position', [100, 100, 1000, 400]);

% 화살표 플롯
subplot(1, 2, 1);
quiver(x, y, u, v, 'b');
title('Vector Field - Arrow Plot');
xlabel('x');
ylabel('y');
axis equal tight;
grid on;

% 스트림라인 플롯
subplot(1, 2, 2);
streamslice(x, y, u, v, 'r');
title('Vector Field - Streamline Plot');
xlabel('x');
ylabel('y');
axis equal tight;
grid on;

% 전체 그림 제목
sgtitle('Visualization of Vector Field F(x,y) = [y, -x]', 'FontSize', 16);

% 벡터장의 회전(curl) 계산
[curlZ] = curl(x, y, u, v);

% 회전 등고선 추가
hold on;
contour(x, y, curlZ, 'k');
colorbar;
title('Vector Field - Streamline Plot with Curl');
```