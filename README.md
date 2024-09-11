# OhhhhhSheep

This project aims to implement a game written in C, involving logic systems, and can be projected on microprocessors (DE-SoC). The demo videos can be found here: [Level 1](https://youtu.be/LwCiuuQ9pLg?si=qxeocj9aRXqseNop), [Level 2 with voice over introduction](https://youtu.be/n2Uc37eJrPM?feature=shared).

Our team developed a matching game inspired by the game OH!Sheep!. First of all, the starter layout has different tiles with various icon laying on top of each other in specific order. This game prompts users to select elements and put them into the basket with limited space of 7 tiles. Elements will overlay on each other, so we can only select the tiles on the surface level. Users can unlock tiles on the bottom layer by clearing the tiles on the top of them. Once the number of elements with the same icon reaches 3, they will cancel each other. [Example video](https://www.youtube.com/watch?v=lQOBAuz5b60). See Appendix A for details.

Aside from the complicated algorithm from the original game, we develop a unique background music and graphic pattern for 7 different icons.

We include 2 level designs:
1. The first is an intro-level design to help users get familiar with the rules, which includes 18 blocks and two layers in total. 
2. The second level is an advanced level that includes 3 layers and 93 icons laying in the shape of ECE. See appendix B for level design specification. 

Inputs and outputs
* Input- PS2 keyboard control:
  * User can use ‘W’ or ‘S’ to opt for next/previous available icon
  * Click ‘ENTER’ to drag the tile to the basket
* Output- Audio
  * A 1-minute background music for the first level
    * When an icon is dragged, the background music is slowed down
  * A 0.5-second audio when you click ‘ENTER’ for the second level (interrupt)
* Output- LED:
  * LED display for the hex-code when an instruction from keyboard is activated
* Output- VGA screen:
  * VGA display of the level
  * Example:
![Screenshot 2024-09-11 140246](https://github.com/user-attachments/assets/9c1fa36c-2f11-45ff-8bb0-21e2d94b4f27)
![Screenshot 2024-09-11 140224](https://github.com/user-attachments/assets/5939c145-4f5f-455d-9315-5f50e056a3a9)

Appendix A: Primary features
![Screenshot 2024-09-11 140205](https://github.com/user-attachments/assets/f5518608-c736-4a30-8cfd-67d656079a1a)

Appendix B: Level design
![Screenshot 2024-09-11 140143](https://github.com/user-attachments/assets/2074cbc5-0035-4a94-babb-b836707ad561)
![Screenshot 2024-09-11 140135](https://github.com/user-attachments/assets/518f0f9f-3630-4c70-8993-7cc777d13785)
