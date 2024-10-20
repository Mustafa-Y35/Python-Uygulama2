# Python-Uygulama2
# Minimum Öklid Mesafesinin Hesaplanması

points = [(2, 3), (4, 1), (-1, -3), (5, 8), (0, 0)]
distances = []

import math

def euclideanDistance(points1,points2):
    return math.sqrt((points1[0] - points2[0]) ** 2 + (points1[1] - points2[1]) **2)

for i in range(len(points)):
    for j in range(i+1,len(points)):
        distance = euclideanDistance(points[i],points[j])
        distances.append(distance)

print(f"Minimum mesafe: {min(distances)} ")
