#GRAPH
05. 인접행렬, 모든 정점 사이에 간선이 존재하므로 인접 리스트보다 인접 행렬로 간선 존재 여부를 확인하는 게 더 효율적이다. <br>
06. 인접리스트, 드물게 간선이 존재하므로 인접 행렬을 사용할 경우 불필요한 메모리가 많아진다. 때문에 인접 리스트가 더 낫다. <br>
08. 간선 제시 순서대로 인접 리스트를 만들면 1-2-3-5-4-6 이다. 때문에 DFS(1)은 1번 호출된다. <br>
12-(1). <img width="2160" height="1168" alt="Image" src="https://github.com/user-attachments/assets/470ffd6e-6c24-4dfe-9924-400768316073" /> <br>
12-(2). <img width="2160" height="1075" alt="Image" src="https://github.com/user-attachments/assets/5b190ecd-4c2c-484c-ac2a-f66f8acb66d2" /> <br>
16. 가능한 위상 정렬 순서는 4가지이다. a-b-c-d-e-f-h-g 혹은 a-d-e-b-c-f-h-g 혹은 a-b-d-c-e-f-h-g 혹은 a-d-b-e-c-f-h-g이다. <br>
create STACK <br>
create visited <- false <br> 
for each vertex v <br>
    if not visited[v] <br>
        DFS(v, visited, STACK) <br>
while not empty(STACK) <br>
    pop(STACK) <br>
DFS(v, visited, STACK) <br>
  visited[v] <- true <br>
  for i in Adj[v] <br>
    if not visited[i] <br>
        DFS <br>
  STACK.push(v) <br>
17. <img width="1644" height="1368" alt="Image" src="https://github.com/user-attachments/assets/5dc14153-5609-4d46-80ca-24cd1e378d1e" /> <br>
18. <img width="643" height="424" alt="Image" src="https://github.com/user-attachments/assets/88be494e-9b95-4c6f-9924-80820335ff14" /> <br>
22. 음의 사이클이 있는 경우이다. <br>
#SORTING
05-(1). <img width="1262" height="1137" alt="Image" src="https://github.com/user-attachments/assets/cfbb9a33-eb9a-4f0c-aa87-138423950045" /> <br>
05-(2). <img width="726" height="1155" alt="Image" src="https://github.com/user-attachments/assets/5204808e-2d38-4a7e-ad72-f2deebdf95f3" /> <br>
05-(3). <img width="1016" height="1088" alt="Image" src="https://github.com/user-attachments/assets/5ff03a9a-0678-4343-9936-b8099fc19f29" /> <br>
06-(1). <img width="875" height="1422" alt="Image" src="https://github.com/user-attachments/assets/0bb8bf85-8bed-4ec5-83af-11b05019b25f" /> <br>
06-(2). <img width="1219" height="580" alt="Image" src="https://github.com/user-attachments/assets/b8642e59-1627-48ab-91e6-03dc6b357dcd" /> <br>
06-(3). <img width="749" height="822" alt="Image" src="https://github.com/user-attachments/assets/cfaeac76-9a0f-4580-98cf-cd713c4329a5" /> <br>
