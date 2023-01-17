# Sign-Up-Form

We have Join Us button, once you click it, it will unfold the page and show up the sign-up form page.


```html
<div class="green-bg">
   <button type="button" >Join Us</button>
</div>
```


```js
signUpBtn.addEventListener('click', () => {
    container.classList.toggle("change");
});
```

```css
.green-bg {
    width: 100%;
    height: 100%;
    background: linear-gradient(to right, #3aaf9f, #4cbf91);
    position: absolute;
    top: 0;
    left: 0;
    z-index: 50;
    transition: width 1.5s cubic-bezier(0.19, 1, 0.22, 1);
}

.container.change .green-bg {
    width: 40%;
}

.signup-form {
    width: 60rem;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0rem;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    padding: 10rem 0;
    transition: left 1.5s cubic-bezier(0.19, 1, 0.22, 1);
}

.container.change .signup-form {
    left: 40rem;
}
```
