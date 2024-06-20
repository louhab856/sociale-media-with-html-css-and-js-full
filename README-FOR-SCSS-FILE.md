@media or  Media queries in CSS , Media query is a CSS technique introduced in CSS3. 
are essential , use by developpers to apply a differents styles to different devices
or screen sizes , to have  : 

==>Responsive Design 💯
==>Optimized User Experience 💯
==>Performance 💯   
==>Accessibility 💯
==>SEO Benefits 💯

# : exemple :
# for the normale width  we have : 
# body {
#  background-color: lightgreen;
# }

# for the   600px width : 
# @media only screen and (max-width: 600px) {
#  body {
#    background-color: lightblue;
#  }
# }
The @mixin directive lets you create CSS code that is to be reused throughout the website.

The @include directive is created to let you use (include) the mixin

# exemple :

# declaring the mixin 
# @mixin bordered($color, $width) {
# border : $width solid $color
# } 

# including the mixin : 

#    myArticle {
#       @include bordered(blue , 1px )
#    }

map-get(map, key)  , Returns the value for the specified key in the map.

# example :  $font-size :("small" : 12 px , "normal" : 18px , "large" : 24px)
# map-get($font-sizes, "small") the result would be 12px 


map-has-key(map, key) , Checks whether map has the specified key. Returns true or false

# example : $font-sizes: ("small": 12px, "normal": 18px, "large": 24px)
# map-has-key($font-sizes, "big")
# the result would be false 

map-keys(map)  , Returns a list of all keys in map.

# $font-sizes: ("small": 12px, "normal": 18px, "large": 24px)
# map-keys($font-sizes)
# the result would be "small", "normal, "large"

map-merge(map1, map2) , Appends map2 to the end of map1.

the @forward is often associated  with Sass , which is css preprocessor , its used to create modules
Sass modules allow u to split ur styles smaller resuable piecess , to be more specific , here is a example : 
# lets say that"s u have _breakpoints.css file , containe the media query breakpoints using mixins
# to include this mixins in anather sass file , u can juste use the keyword : @forward
# i should put in mind that"s 16 pixls is equale to 1 rem
