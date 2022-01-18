# 100 Days Of Code - Log

### Day 0: January 17, 2022 
<!-- ##### () -->

**Today's Progress**: Completed trillo project of [Advanced CSS and Sass Course](https://www.udemy.com/course/advanced-css-and-sass/?src=sac&kw=advance+css+and+sass)

**Thoughts:** It was Amazing to do the Project. I learned Lot About Css FlexBox. Property I learned during this was Mask-image, mixins is sass, Proper user of flex grow,shrink,basis,etc.

**Link to work:** [Project Final Repo](https://github.com/Chandraprakash-Darji/Trillo-Final-Advanced-CSS-and-Sass-Course)

### Day 0: January 18, 2022 
<!-- ##### () -->

**Today's Progress**: Learned About Css Grid from [Advanced CSS and Sass Course](https://www.udemy.com/course/advanced-css-and-sass/?src=sac&kw=advance+css+and+sass)

**Thoughts:** Grids are amazing to arrange layout on webpage.

**Properties I learned:** 
```css
body{
    display: grid;
    grid-template-columns: 150px 1fr;    // 1fr is awailable space
    grid-template-rows: repeat(2, 150px) 300px;   // 150px 150px 300px

    grid-row-gap: 30px;
    grid-column-gap: 30px;

    grid-gap: 30px;


    grid-row-start: 2;
    grid-row-end: 3;
    grid-row:  2 / 3;  //  grid-row-start: 2;  grid-row-end: 3;

    grid-column-start: 2;
    grid-column-end: 3;
    grid-column: 2 / 3;  //     grid-column-start: 2;   grid-column-end: 3;

    grid-area: 2 / 2 / 3 / -1;   //   grid-row:  2 / 3;    grid-column: 2 / 3; 
    // -1 indicates last column/row line
    grid-column: 1 / span 3;  // it will span 3 from 1 
}

```
**What I learned and Created:** 
```html 
 <div class="grid">
            <div class="grid__head">Header</div>
            <div class="grid__sm-box--1">Small Box 1 </div>
            <div class="grid__sm-box--2">Small Box 2 </div>
            <div class="grid__sm-box--3"> Small Box 3</div>
            <div class="grid__side-bar">SideBar</div>
            <div class="grid__main">Main Content</div>
            <div class="grid__footer">Footer</div>
        </div>
```
```css
    .grid{
    display: grid;
    color: #eee;
    font-family: sans-serif;
    
    width: 50%;
    margin: 0 auto;
    grid-template-columns: 1fr 1fr 1fr 20%;
    grid-template-rows: 40px 120px 400px 40px;
    grid-gap: 30px;

    & > * {
        background-color: red;
        padding: 10px;
    }

    &__head{
        grid-row: 1 / 2;
        grid-column: 1 / -1;
    }

    &__side-bar{
        grid-column: -2 / -1;
        grid-row: 2 / -2;
        // height: 500px;
    }
    &__main{
        grid-row: 3 / 4;
        grid-column: 1 / -2;
    }
    &__footer{
        grid-row: 4 /5;
        grid-column: 1 / -1;
    }
}
```
**Screenshot I Created:** 
![Screenshot](./18-Jan/output.png)