# Flex-Box
an Introduction to Flex-box

					Flex-Direction

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


					Justify-Content
					
'justify-content' can be used to determine the spacing between each element of a flex-box.
#container{
	justify-content: boblawblah;
}
There are several different options to 'justify-content' starting with "no pun intended" flex-start
#container{
	justify-content: flex-start;
}
'flex-start' will align the items to the left side of the container.  don't get this confused with flex-direction row and the next one will show you why
#container{
	justify-content: flex-end;
}
'flex-end' will push all the elements to the right BUT the elements will remain in the order that they are listed in the markup.  
then there's 
#container{
	justify-content: center;
}
this one has got to be my favorite.  The center option does what?
These next two are neat
#container{
	justify-content: space-between;
]
what 'space-between' does is puts space between the elements and only the elements so the first element will hug the left container border and the right element will hug the right container border.  
now if you want space around each element then...
#container{
	justify-content: space-around;
}
Someone has already thought of you and your concerns.  'space-around' puts space around each element, even the left-most and right-most elements buuuuuuuuuut!!!  the space on the left side of the left-most element and the space on the right side of the right-most element are a bit smaller then the space between the other elements.  to avoid this you may want to use
#container{
	justify-content: space-evenly;
}
which puts an even amount of space on both sides of each element.

Keep in mind the setting of 'flex-direction' when using 'justify-content' as it will affect how the content gets placed

						Flex-Wrap
						
'flex-wrap'
A delicious wrap made with Turkey, Bacon, Tomatoe, Colby-Jack cheese, Jalapenos and peppercinis all covered in a chipotle aioli sauce and topped with crunchy corn chips.  
no that's not 'flex-wrap' it is lunch time and i am getting quite hungry
#container{
	flex-wrap: wrap;
}
will maintain the size of each element no matter what the size of the container is but it will move the elements in a fashion that they all fit within the container whilst keeping their original size perserved.  
	There is also 'wrap-reverse' and 'nowrap' incase you have already had lunch
	
						Align-Items

'align-items' will align the items along the X axis
and you can choose from options like 'start' 'end' 'flex-start' 'flex-end' 'center' 'baseline' which are all pretty self explanatory
