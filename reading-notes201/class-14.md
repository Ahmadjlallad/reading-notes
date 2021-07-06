# CSS Transforms, Transitions, and Animations

## Transitions

- remended pseudo-classes to make Transitions `:hover`, `:focus`, `:active`, and `:target` `transition`.

- Vendor Prefixes Simply put, vendor prefixes are a way for your browser to support new CSS features before they become fully supported in all browsers.

- The Transition property

```CSS
{transition-property: border;
/* property that will get transitioned*/
transition-duration: 150ms;
/* takes a numerical value with ms or s unit */
transition-timing-function: esse;
/* Transition Timing set the speed in which a transition will move.*/
/* transition:Shorthand ; */
}
```

but not all properties can be transitioned search [MDN Animatable CSS properties](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties)

- `@keyframes` set multiple point for the transition like `0% and 100%` for `from{} to{}` from and to equal to 0% & 100%.

```css
@keyframes mymove {
  0% {
    top: 0px;
  }
  25% {
    top: 200px;
  }
  50% {
    top: 100px;
  }
  75% {
    top: 200px;
    100% {
    }
    top: 0px;
  }
  /* used with animation property*/
}
```

- `animation` property

```css
{
    animation-name @keyframes
    /* name of the keyframe */
animation-duration
/* takes a numerical value with ms or s unit */
animation-timing-function
/* speed curve of the animation */
animation-delay
/* delay before the animation will start */
animation-iteration-count
/* how many times you want the animation to play */
animation-direction
/* direction reverse or not */
animation-fill-mode
/* specify what will happen after the animation end  */
animation-play-state
/* running or paused */
/* Shorthand Animations */
}
```

```css
 {
  transform: scale(x, y);
  /* change the size of the element */
  transform: translate();
  /* Moves an element sideways or up and down. */
  transform: rotate(x, y, z);
  /* Rotates the element clockwise from its current position. */
}
```

# working as group

- Norms the study refer it to be important than other catagories
  - Our meetings will begin and end on time.
  - We will listen to each other and not interrupt.
  - We will make sure everyone has had a chance to speak.
  - We will support our facilitator's efforts to moderate discussions.
  - We will avoid ethnic or gender-based humor.
  - We will speak respectfully to each other.
  - adopt new norms like having deferent conversation or talk about what intrusts you and ask what interests the group.
  - also they mention psychological safety.
