# Dice Roll Circuit

> This project is designed for the DE10-Lite. It uses the 6 switches located at the bottom of the board as well as the 2 buttons located directly above those. The 6 switches on the bottom correspond to the 6 seven-segment displays on the righthand side.
> 
> The program works by turning on (up position) the switch corresponding to the 7seg displays you'd like to roll and then pressing the bottom button. The animation will then snap to a number, representing the value that has been rolled (same for all). To reset the 7seg, a similar process is employed. Switch on the displays to reset, and push the reset button.
>
> The numbers are randomly generated through a 4-bit linear feedback shift register. The shift register is built for 7 numbers, so when a "7" gets processed it is instead immediately rolled over to a 3. The full sequence is `1736524`, which gets augmented to `136524`.
>
> An extremely detailed breakdown of the circuit's logic (with provided pictures and SystemVerilog code is provided in the pdf found in the repository.
