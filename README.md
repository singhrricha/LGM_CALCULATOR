# LGM_CALCULATOR
The calculator I built allows users to perform basic mathematical operations such as addition, subtraction, multiplication, and division. It also includes the ability to delete a number, clear the calculator, and display the result of a calculation.

To create this calculator, I utilized an object-oriented approach, which involved creating a class that defines the behavior and properties of the calculator. The class is called "Calculator" and is instantiated with two arguments, "previousOperandTextElement" and "currentOperandTextElement". These two elements correspond to the previous and current operand display areas in the calculator UI.

The "Calculator" class contains methods that enable the calculator to perform its functions. The first method, "clear", sets the current operand, previous operand, and operation to undefined. The second method, "delete", removes the last digit of the current operand if it is not empty. The third method, "appendNumber", adds a number or a decimal point to the current operand if the user clicks a number button or a decimal button.

The fourth method, "chooseOperation", sets the current operation and the previous operand when the user clicks an operation button such as addition, subtraction, multiplication, or division. If the previous operand is not empty, it performs the computation before setting the operation and the previous operand to the new values.

The fifth method, "compute", performs the computation of the two operands based on the selected operation. It then sets the current operand to the computed value and sets the operation and previous operand to undefined.

The sixth method, "getDisplayNumber", formats the number to be displayed in the UI. If the number has decimal places, it formats it to show the integer digits and the decimal digits. If the number does not have decimal places, it formats it to show only the integer digits.

The final method, "updateDisplay", updates the display of the calculator by setting the text of the current operand and the previous operand to the corresponding values using the "getDisplayNumber" method.

To create the UI, I used HTML and CSS to structure and style the calculator layout. I then utilized JavaScript to add functionality to the UI by adding event listeners to the number buttons, operation buttons, and delete button. These event listeners trigger the appropriate methods in the "Calculator" class, which in turn update the display of the calculator.
