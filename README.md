# Flex-Box
an Introduction to Flex-box

The way the divs are setup are from top to bottom so they display from top to bottom like a pringles can of chips.  
When adding the display property to container and setting it to flex, adheres the flex-box framework and makes the divs line up inline side by side.

#container{
	display: flex;
}

This can be changed up a bit with the 'flex-direction' property

#container{
	flex-direction: row;
}

by setting it to row nothing really changes because the left to right direction is by default, but if we change it to row-reverse

#container{
	flex-direction: row-reverse;
}

 then the elements get displayed from right to left.

There is also 'column' and 'column-reverse'.
'column'

#container{
	flex-direction: column;
}

displays the elements from top to bottom, again like the pringles can of chips.
and 'column-reverse' displays them from bottom to top

#container{
	flex-direction: column-reverse;
}

!!!--NOTE--!!!
	If the elements are to big to all fit within the container provided for them then they will each be squished in by making each element smaller until they are all the same size and they all fit.  for example say you have 4 elements and each element is 100px but they all need to fit into a 100px container.  Well that is just not going to happen right.  By using flexy-box then it will reduce the size of each element to 25px making the total size of all four elements 100px to fit within the container.  Flex-box does this automatically so you don't have to worry about the math.
	if each element was say 10px big then there would be a void of extra space within the container.
