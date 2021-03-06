# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [The challenge](#the-challenge)
- [Screenshot](#screenshot)
- [Links](#links)
- [What I learned](#what-i-learned)
  - [Challenges](#challenges)
  - [Proud Moment](#proud-moment)
- [Author](#author)

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size.
- See hover states for interactive elements.

### Screenshot

![Screenshot](screenshot.JPG)

### Links

- Solution URL: [Solution URL](https://github.com/dheerajmnk/frontendmentor-challenges/tree/main/nft-preview-card-component)
- Live Site URL: [Live Site URL](https://dheerajmnk.github.io/frontendmentor-challenges/nft-preview-card-component/index.html)


### What I learned

#### Challenges

1. Adding an overlay image for the equilibrium seemed to be pretty difficult for me. I managed to get it done after learning more about relative-absolute positioning. But there was still a problem to be fixed

![1a](misc/1a.JPG)

My view icon was not at the centre of the equilibrium. This was odd because I used 50% relative positioning for both front and top. After googling for a while, I learnt about the transform property.

```css
transform: translate(-50%, -50%);
```

This did the trick.

![1b](misc/1b.JPG)

2. I was not able to get my text element centered properly beside the avatar.

![2](misc/2.JPG)

I was pretty sure that I could not achieve this without knowing advanced concepts of flexbox and grid. I discovered a property called align-items that could be a given a value of center. This property could only be used on flex items so I had to change its display to flex.

```css
.creation {
    display: flex;
    align-items: center;
}
```

#### Proud Moment

When I saw this part of the required design, I knew I could achieve it with ease. 

![3](3.JPG)

I managed in doing so, just with my knowledge of inline-block display and padding.

```css
.info .eth{
    color: hsl(178, 100%, 50%);
    display: inline-block;
    padding-right: 40px;
}

.info .eth p{
    display: inline-block;
    padding-left: 5px;
}

.info .days{
    color: hsl(215, 51%, 70%);
    display: inline-block;
    padding-left: 40px;
}

.info .days p{
    display: inline-block;
    padding-left: 5px;
}
```

### Author

- Frontend Mentor - [@dheerajmnk](https://www.frontendmentor.io/profile/dheerajmnk)
- Twitter - [@dheerajmnk](https://www.twitter.com/dheerajmnk)
