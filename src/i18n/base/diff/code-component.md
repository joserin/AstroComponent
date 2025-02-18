```astro
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaultClass='aspect-video';
const { class: className = defaultClass, ...rest } = Astro.props;
---

<div class="container">
  <div class={className}>
      <slot name="first-image"/>
      <slot name="second-image"/>
  </div>
  <input type="range" min="0" max="100" value="50" aria-label="Percentage of before photo shown" class="slider"/>
  <div class="slider-line" aria-hidden="true"></div>
  <div class="slider-button" aria-hidden="true">
    <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" viewBox="0 0 256 256">
      <rect width="256" height="256" fill="none"></rect>
      <line x1="128" y1="40" x2="128" y2="216" fill="none" stroke="currentColor" stroke-linecap="round" 
        stroke-linejoin="round" stroke-width="16"></line>
      <line x1="96" y1="128" x2="16" y2="128" fill="none" stroke="currentColor" stroke-linecap="round" 
        stroke-linejoin="round" stroke-width="16"></line>
      <polyline points="48 160 16 128 48 96" fill="none" stroke="currentColor" stroke-linecap="round" 
        stroke-linejoin="round" stroke-width="16"></polyline>
      <line x1="160" y1="128" x2="240" y2="128" fill="none" stroke="currentColor" stroke-linecap="round" 
        stroke-linejoin="round" stroke-width="16"></line>
      <polyline points="208 96 240 128 208 160" fill="none" stroke="currentColor" stroke-linecap="round" 
        stroke-linejoin="round" stroke-width="16"></polyline>
    </svg>
  </div>
</div>
```