# Slots/Redemption Games IO Board
This board comes with 4P/6P/8P/12P variations.
## Joystick connectors (CON13-CON22)
Assuming notches on the connectors are facing downwards.
### Pin arrangement
<table>
    <tr>
        <td>2</td><td>4</td><td>...</td><td>26</td>
    </tr>
    <tr>
        <td>1</td><td>3</td><td>...</td><td>25</td>
    </tr>
<table>

### Pin definition
(I: input, O: output)
<table>
    <tr>
        <td>I</td><td>I</td><td>I</td><td>I</td><td>O</td><td>O</td><td>O</td><td>O</td>
    </tr>
    <tr>
        <td>Joystick down</td>
        <td>Jotstick left</td>
        <td>Fire button</td>
        <td>Attendant manual cash in key switch [^1]</td>
        <td>Hopper conter-clockwise signal</td>
        <td>Hooper feedBack singal</td>
        <td>Hopper clockwise signal</td>
        <td>Bet change button light</td>
        <td>+12V</td>
        <td>+12V</td>
        <td>GND</td>
        <td>GND</td>
        <td>GND</td>
        <td>GND</td>
    </tr>
    <tr>
        <td>Joystick up</td>
        <td>Jotstick right</td>
        <td>Bet change button</td>
        <td>Coin signal</td>
        <td>Attendant hand pay key switch [^1]</td>
        <td>Ticket printer error signal</td>
        <td>Ticket printer trigger signal</td>
        <td>Fire button light</td>
        <td>+12V</td>
        <td>+12V</td>
        <td>+5V</td>
        <td>GND</td>
        <td>GND</td>
        <td>GND</td>
    </tr>
    <tr>
        <td>I</td><td>I</td><td>I</td><td>I</td><td>I</td><td>O</td><td>O</td><td>O</td>
    </tr>
</table>
[^1]: These switches are marked as "key in/key out" which are too vague. These key switches are inside the cabinet and directly adds/subtracts certain amounts of credits from player's bankroll for attendents doing [hand pay](https://en.wikipedia.org/wiki/Hand_pay)/manual cash in.


## 24V Input
Assuming the bulge of the connector is facing upwards.
<table>
<tr>
    <td>GND</td><td>+12V</td>
</tr>
<tr>
    <td>GND</td><td>GND</td>
</tr>
</table>

## Counter Connector (CON6)
Assuming the notch of the connector is facing downwards.

All pins are for output.
<table>
<tr>
    <td>TEST4?</td>
    <td>TEST3?</td>
    <td>TEST2?</td>
    <td>TEST1?</td>
    <td>Counter D</td>
    <td>Counter C</td>
    <td>Counter B</td>
    <td>Counter A</td>
    <td>+12V</td>
</tr>
</table>

## Bill Accepter Connector (CON8/CON10)
Assuming the notch of the connector is facing downwards.

All pins are for input.
### CON8
<table>
<tr>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>?</td>
    <td>?</td>
    <td>?</td>
    <td>?</td>
    <td>?</td>
    <td>?</td>
    <td>10P Credit Relay signal</td>
    <td>9P Credit Relay signal</td>
</tr>
</table>

### CON10
<table>
<tr>
    <td>8P Credit Relay signal</td>
    <td>7P Credit Relay signal</td>
    <td>6P Credit Relay signal</td>
    <td>5P Credit Relay signal</td>
    <td>4P Credit Relay signal</td>
    <td>3P Credit Relay signal</td>
    <td>2P Credit Relay signal</td>
    <td>1P Credit Relay signal</td>
</tr>
</table>

## Joystick Lamp Connector (CON7)
Assuming the notch of the connector is facing downwards.

All pins are for output.

This connector is for joysticks with bulit-in lamp. It could be left empty if there aren't corresponding lamps.
<table>
<tr>
    <td>-</td>
    <td>10P joystick lamp</td>
    <td>9P joystick lamp</td>
    <td>8P joystick lamp</td>
    <td>7P joystick lamp</td>
    <td>6P joystick lamp</td>
    <td>5P joystick lamp</td>
    <td>4P joystick lamp</td>
    <td>3P joystick lamp</td>
    <td>2P joystick lamp</td>
    <td>1P joystick lamp</td>
</tr>
</table>

## Test Button (CON9)
Assuming the notch of the connector is facing downwards, and the rightmost pin is 1.

All pins are for input.
<table>
<tr>
    <td>GND</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>Test button</td>
</tr>
</table>

## RS485 - Wiring to the RJ11 on the GP1 board
Assuming the bulge of the connector on the IO board is facing leftwards, cutouts facing rightwards, and the upmost pin is 1. 
Assuming the bulge of the connector on the GP1 board is facing rightwards, and the upmost pin is 1.
<table>
<tr>
    <th>IO side</th>
    <td>1</td>
    <td>3</td>
</tr>
<tr>
    <th>GP1 side</th>
    <td>3</td>
    <td>4</td>
</tr>
</table>

## Coin Out Button Connector (CON11)
Assuming the notch of the connector is facing downwards, and the rightmost pin is 1.

All pins are for input.
<table>
<tr>
    <td>10P coin out button</td>
    <td>9P coin out button</td>
    <td>8P coin out button</td>
    <td>7P coin out button</td>
    <td>6P coin out button</td>
    <td>5P coin out button</td>
    <td>4P coin out button</td>
    <td>3P coin out button</td>
    <td>2P coin out button</td>
    <td>1P coin out button</td>
</tr>
</table>

# Slots/Redemption Games Hopper Relay board
## Input (JP1)
Assuming the notch of the connector is facing leftwards.

All pins are for input.
<table>
<tr><td>GND</td></tr>
<tr><td>+12V</td></tr>
<tr><td>Counter-clockwise signal</td></tr>
<tr><td>Clockwise signal</td></tr>
</table>

## Output (JP2)
Assuming the notch of the connector is facing leftwards.

All pins are for output.
<table>
<tr><td>Motor-</td></tr>
<tr><td>Motor+</td></tr>
<tr><td>+24V</td></tr>
<tr><td>GND</td></tr>
</table>
