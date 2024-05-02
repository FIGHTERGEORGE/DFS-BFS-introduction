# DFS-BFS-introduction
depth first search / breadth first search
Personal records dfs and bfs, which can be used as reference and learning materials..
<img width="233" alt="微信图片_20240502220417" src="https://github.com/FIGHTERGEORGE/DFS-BFS-introduction/assets/167811390/1ddad9bb-891e-4e6a-b107-5d639d5655d1">


****BFS****---------------------------------------------------------------------------------------


Add ‘0’ to queue,add ‘0’ to visited..
QUEUE: 0
VISITED: 0

Pop ‘0’ from queue.
Add elements adjacent to ‘0’ which are ‘1’, ’2’ , ‘3’ to queue
And mark ‘1’, ’2’, ’3’ visited.
QUEUE: 123
VISITED: 0123

Pop ‘1’ from queue.
Adjacent elements ‘0’ and ‘2’ are in visited.
Don’t need to add any new value to the queue.
QUEUE: 23
VISITED: 0123

Pop ‘2’ from queue.
Adjacent elements are ‘6’ and ‘3’.
Since ‘3’ has been in visited, we add ‘6’ to the queue and mark ‘6’ as visited.
QUEUE: 36
VISITED : 01236

Pop ‘3’ from queue.
Adjacent elements are ‘2’, ‘4’, ‘5’. 
‘2’ is in visied. 
We just add ‘4’, ‘5’ to the queue.
QUEUE: 654
VISITED: 0123654

Similarly:
QUEUE: 547
VISITED: 01236547

Similarly:
QUEUE: 478
VISITED: 012365478

Similarly:
Pop ‘4’
Then pop’7’, then pop ‘8’

Finally: 
VISITED: 012365478

FOR CODING:
CHESSBOARD TRAVERSAL (python)
---------------------------------------------------------------------------


<img width="233" alt="微信图片_20240502220417" src="https://github.com/FIGHTERGEORGE/DFS-BFS-introduction/assets/167811390/5669a7d9-3d99-4a35-b19e-de8432c3be35">


****DFS****--------------------------------------------------------------

ADD ‘0’ to the stack.
STACK: 0
VISITED: 

Pop ‘0’ from the stack, add ‘0’ to the visited.
Add adjacent elements to stack.
STACK: 123
VISITED: 0

Pop ‘3’, mark it as visited.
Add adjacent elements to the stack which are ‘4’, ‘5’
Since ‘0’ is in visited and ‘2’ is in stack we don’t add them to stack.
STACK: 1245
VISITED: 03

Pop ‘5’, mark visited
Add adjacent elements to stack which is ‘8’
Since ‘4’ is in stack and ‘3’ is in visited we don’t add them
STACK: 1248
VISITED: 035

Similarly, pop ‘8’ from stack..
STACK: 1247
VISITED: 03587

Similarly,
STACK: 1246
VISITED: 03587

Then,
STACK: 124
VISITED: 035876

Then,
STACK: 12
VISITED: 0358764

Then,
STACK: 1
VISITED: 03587642

Then,
STACK: 
VISITED: 035876421
-----------------------------------------------------------------------------







