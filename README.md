# svg-social-media-rounded-bar

Font awesome is the Internet's icon library and toolkit, used by millions of designers, developers, and content creators.
But all of that come with a cost, 131k is the size of "fontawesome.all.css" for the last version of Font awesome (6.2.0)
the question is, why should I request all of the icons in fontawesome.all.css when I only need some of them?

and the answer is not, you should not, why not request only the icons that you need?

## My solution for that is creating my own collection of icons , and guess what? 

✓ It's very easy to use

✓ It's very easy to maintain

✓ You can use in html and JavaScript (no bundler or extra packages required)

✓ Add only you won't to use in each project

✓ it's free and open source

✓ And the most important, very slim (1k≈ by icon)

All of that is done using SVGs

## What is SVG?

SVG (Scalable Vector Graphics) is an image format for vector graphics.
What advantage give as SVGs?

✓ Small file sizes that compress well

✓ Scales to any size without losing clarity

✓ Looks great on retina displays

✓ Design control like interactivity, filters and colors

SVG looks like html, take a look at this icon

``` <svg width="100" height="100" alt="email" aria-hidden="true" data-prefix="fal"
data-icon="envelope" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"
class="svg-inline--fa fa-envelope fa-w-16 fa-7x">
<path fill="white"
d="M464 64H48C21.5 64 0 85.5 0 112v288c0 26.5 21.5 48 48 48h416c26.5 0 48-21.5 48-48V112c0-26.5-21.5-48-48-48zM48 96h416c8.8 0 16 7.2 16 16v41.4c-21.9 18.5-53.2 44-150.6 121.3-16.9 13.4-50.2 45.7-73.4 45.3-23.2.4-56.6-31.9-73.4-45.3C85.2 197.4 53.9 171.9 32 153.4V112c0-8.8 7.2-16 16-16zm416 320H48c-8.8 0-16-7.2-16-16V195c22.8 18.7 58.8 47.6 130.7 104.7 20.5 16.4 56.7 52.5 93.3 52.3 36.4.3 72.3-35.5 93.3-52.3 71.9-57.1 107.9-86 130.7-104.7v205c0 8.8-7.2 16-16 16z"
class="">
</path>
</svg> ```

## Browser support
If you check in Caniuse, SVG is supported by all modern browsers.
Using SVG

✓ You can use svg as <img>

```<img src="email.svg" alt="email icon">```

✓ You can use as an <object>
  
```
<object type="image/svg+xml" data=""email.svg" class="email">
  Email <!-- fallback image in CSS --> 
</object>```
                                                            
## My approached of using SVGs
we have a directory that contain all svg files , index.hmtl file, style.css file.
Where a get these SVGs?
simply got to this Github repository: Fontawesome-svgs and copy all SVGs that you won't
then past the svg code in a file with svg extention
for exemple:
                                                            
✓ copy the email svg code
                                                            
✓ add width="100" height="100"
                              
✓ change alt value to "email"
                             
✓ change the value of fill to "white"
                                     
the starting code of the SVG:
                                     
```<svg aria-hidden="true" data-prefix="fal" data-icon="envelope" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" class="svg-inline--fa fa-envelope fa-w-16 fa-7x"><path fill="currentColor" d="M464 64H48C21.5 64 0 85.5 0 112v288c0 26.5 21.5 48 48 48h416c26.5 0 48-21.5 48-48V112c0-26.5-21.5-48-48-48zM48 96h416c8.8 0 16 7.2 16 16v41.4c-21.9 18.5-53.2 44-150.6 121.3-16.9 13.4-50.2 45.7-73.4 45.3-23.2.4-56.6-31.9-73.4-45.3C85.2 197.4 53.9 171.9 32 153.4V112c0-8.8 7.2-16 16-16zm416 320H48c-8.8 0-16-7.2-16-16V195c22.8 18.7 58.8 47.6 130.7 104.7 20.5 16.4 56.7 52.5 93.3 52.3 36.4.3 72.3-35.5 93.3-52.3 71.9-57.1 107.9-86 130.7-104.7v205c0 8.8-7.2 16-16 16z" class=""></path></svg>```

the final code of svg

```<svg width="100" height="100" alt="email" aria-hidden="true" data-prefix="fal"
data-icon="envelope" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"
class="svg-inline--fa fa-envelope fa-w-16 fa-7x">
<path fill="white"
d="M464 64H48C21.5 64 0 85.5 0 112v288c0 26.5 21.5 48 48 48h416c26.5 0 48-21.5 48-48V112c0-26.5-21.5-48-48-48zM48 96h416c8.8 0 16 7.2 16 16v41.4c-21.9 18.5-53.2 44-150.6 121.3-16.9 13.4-50.2 45.7-73.4 45.3-23.2.4-56.6-31.9-73.4-45.3C85.2 197.4 53.9 171.9 32 153.4V112c0-8.8 7.2-16 16-16zm416 320H48c-8.8 0-16-7.2-16-16V195c22.8 18.7 58.8 47.6 130.7 104.7 20.5 16.4 56.7 52.5 93.3 52.3 36.4.3 72.3-35.5 93.3-52.3 71.9-57.1 107.9-86 130.7-104.7v205c0 8.8-7.2 16-16 16z"
class=""></path>
</svg>```

save the file "email.svg" to the directory "./svgs"
then add your SVG to index.html
                                                   
```
<div class="social email">
<object class="svg-container" type="image/svg+xml" data="/svgs/email.svg">Email</object>
</div>
```


as you can see SVG is added to an <object> html tag with data attribute that point to the svg file, with css class "svg-container" that gives a fixed height and width to the svg.

```.svg-container {
width: 30px;
height: 30px;
padding: 8px;
}```
                                                                                                                                  
all is wraped around a div with two classess: "social" and "email"
```.social {
margin: 5px;
border-radius: 50%;
box-shadow: 0 3px 10px rgb(0 0 0 / 0.3);
transition: all .1s ease-in-out;
}
.social:hover {
opacity: 0.7;
transform: scale(1.1);
}```
                                                                  
that gives a circle shape to the icon with two animations on hover ( opacity and scale)
for the css class "email"
                         
```                        
.email {
background-color: #807f7f;
}
```
                         
with give a unique background color.
                         
the size of each svg file is approximately 1k , compared to the 131k of the font awesome (v 6.2.0 )
