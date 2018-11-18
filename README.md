# Trello-color-palette
Scss (sass) and css trello color palette to use in your next project. 

![Image](https://i.imgur.com/4k7bv8I.png)

## Customization
Use sass file to create your custom class names 
sass file orgnized into three parts/steps

 1. Defining all colors and turn the colors to variables
``` 
$Trello-Blue-50  :  #E4F0F6;
```
 2. Turn color variables to a color map
``` 
$color-map: (
	Blue-50 : $Trello-Blue-50,
)
```
 3. Using map turn all colors to background-color, Color and
 border-color with the same name
``` 
@each $color-key, $color-var in $color-map {
	.trello-bg--#{$color-key} {
		background-color: $color-var;
	}
}
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTg4NTA4NzI5NywtMTg3MzI0MjA2Nl19
-->