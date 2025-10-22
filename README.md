# mataplotlib
import matplotlib.pyplot as plt
import numpy as np

# 각도를 위한 t 값
t = np.linspace(0, 2 * np.pi, 1000)

# 하트 방정식 (x, y 좌표)
x = 16 * np.sin(t)**3
y = 13 * np.cos(t) - 5 * np.cos(2*t) - 2 * np.cos(3*t) - np.cos(4*t)

# 그래프 그리기
plt.figure(figsize=(6,6))
plt.plot(x, y, color='red', linewidth=2)
plt.fill(x, y, color='pink', alpha=0.6)  # 하트 안 채우기

# 배경 없애기
plt.axis('off')
plt.title("❤️ 하트 모양 그래프", fontsize=16)
plt.show()
