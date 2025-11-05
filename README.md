# CIS 5660 HW04 Procedural Buildings

## Final Render and Video

<img width="1280" height="720" alt="HouseRender" src="https://github.com/user-attachments/assets/2e741018-cc6c-4b75-83b8-10e3400016ae" />


In this project, I create a procedural building with a surreal, minimalist style in Houdini. Some methods used originate from this [video](https://www.youtube.com/watch?v=uIe97023sDk&t=979s&ab_channel=SimonHoudini ) by Simon Houdini.


https://github.com/user-attachments/assets/ab29e397-eb78-4863-ad2b-e5cbf470a005


## Inspiration

<img width="537" height="620" alt="image" src="https://github.com/user-attachments/assets/786c95d2-e622-49e6-89e5-f6e2a49e6c28" />

https://80.lv/articles/realistic-procedural-architecture-for-games



<img width="990" height="398" alt="Screenshot 2024-10-22 225215" src="https://github.com/user-attachments/assets/b78f3f45-45da-43a2-ae6a-2d342892c719" />

https://www.pixiv.net/en/artworks/121784384



<img width="700" height="394" alt="image" src="https://github.com/user-attachments/assets/bc00ffa8-63b9-44b0-ae5b-54684809ff81" />

Habitat 67



I wanted to create a very irregular piece of architecture that was sharp and geometric in nature. The first image above was my main reference.

## Workflow

One late day used.

I start off with boxes of randomized dimensions, rotations, and offsets, and I stack them on top of one another as distinct floors using a For Loop and a Match Size node.


<img width="536" height="495" alt="Screenshot 2025-11-04 193830" src="https://github.com/user-attachments/assets/12560039-9f7b-47a3-b756-a593eaee7ddf" />


Next, I merge secondary boxes to each main box. I randomize their dimensions similarly but keep their y-dimensions similar to the main box, slightly adjusting the rotation, and offset it from one of the main boxes' faces.


<img width="528" height="497" alt="Screenshot 2025-11-04 193901" src="https://github.com/user-attachments/assets/eaa47477-e212-43cb-988c-63f86eb986ce" />


Using the intersection of a plane with the geometry, I extract the perimeter of each floor, and use the chain node to find appropriate points for placing assets. These points become the locations for my windows, doors, and balconies. A roof is placed on the top-most box.


<img width="526" height="432" alt="Screenshot 2025-11-04 223653" src="https://github.com/user-attachments/assets/a5f2962a-f854-4e5c-a8f1-6189079fdfb9" />


These decoration assets also procedurally made in Houdini and allow for variation through different parameters.


<img width="473" height="488" alt="Screenshot 2025-11-04 194028" src="https://github.com/user-attachments/assets/6c6a679e-9b00-485c-a201-222beaabbb90" />
