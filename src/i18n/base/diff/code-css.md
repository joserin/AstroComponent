```css

<style>
  .container {
    display: flex;
    place-content: center;
    position: relative;
    overflow: hidden;
    border-radius: 1rem;
    --position: 50%;
    width: fit-content;
  }

  .slider {
    position: absolute;
    inset: 0;
    cursor: pointer;
    opacity: 0;
    width: 100%;
    height: 100%;
  }

  .slider:focus-visible ~ .slider-button {
    outline: 5px solid black;
    outline-offset: 3px;
  }

  .slider-line {
    position: absolute;
    inset: 0;
    width: .2rem;
    height: 100%;
    background-color: #fff;
    left: var(--position);
    transform: translateX(-50%);
    pointer-events: none;
  }

  .slider-button {
    position: absolute;
    background-color: #fff;
    color: black;
    padding: .5rem;
    border-radius: 100vw;
    display: grid;
    place-items: center;
    top: 50%;
    left: var(--position);
    transform: translate(-50%, -50%);
    pointer-events: none;
  }
</style>
```