**4 Floor Elevator System
ROBT4456 - Final PLC Project 2025
Damon Park**

**Part 1: Four-Floor Elevator**
Programmed the PLC elevator to respond to calls made from floors 1-4.
• Once run, the elevator moves to the Floor 1 and wait.
• The elevator can be called to a corresponding floor with FPB1, FPB2, FPB3, and FPB4.
• FIL1, FIL2, FIL3, and FIL4 notify the user that the call is accepted.
• The elevator stops at the floor it was called to and wait for the next call.
• The elevator never moves below Floor 1 or above Floor 4.

**Part 2: Inside Panel**
Programmed the PLC elevator to respond to requests to move to one of four floors.
• Passengers can request to go to a corresponding floor with PB1, PB2, PB3, and PB4.
• IL1, IL2, IL3, and IL4 notify the passenger the request is accepted.

**Part 3: Elevator Door**
Programmed the PLC elevator to open and close the elevator door to allow passengers on.
• The elevator door opens for 5 seconds when servicing a floor.
• After 2 seconds, the door can be closed by pressing PBC on the inside panel.
• Pressing PBO holds the door open for another 3 seconds.
• If the elevator is waiting for a floor call, the door remains closed.
• If the elevator is called to the floor, it is already on, the door opens.
• The elevator never move while the door is open.
• Programmmed the door with a separate state machine.

**Part 4: Emergency Stop**
Programmed the PLC elevator to stop in the event of an emergency.
• Pressing the emergency stop button PBE5 stops the operation of the elevator.
• An indicator light ILE5 indicates the elevator has been stopped due to an emergency.
• The elevator does not respond to calls or requests.
• If an emergency occurs with the door open, the door remains open.
• The door will be opened and remain open if the elevator is at a floor.
• A reset pushbutton, START, to be pressed once it is safe.
• After a reset, the elevator returns to the 1st floor with the door closed.

**Part 5: Multiple Calls/Requests**
Programmed the PLC elevator to respond to multiple simultaneous calls or requests for any floor.
• The elevator services each intermediate floor with a pending request/call that is passed.
• The elevator maintains its direction until the highest/lowest request/call is serviced.
• The elevator never repeatedly service two floors ignoring other floors.
