```css

<style>
    .default-circle{
        width: 1.25rem;
        height: 1.25rem;
        border: 0.25rem solid transparent;
        border-top: 0.25rem solid #3498db;
        border-radius: 50%;
        animation: spin 1.2s linear infinite;
    }
    .default-bar {
        width: 2rem;
        height: 0.25rem;
        background-color: #3498db;
        animation: progress 2s linear infinite;
    }
    @keyframes spin {
        0% { transform: rotate(0deg); }
        100% { transform: rotate(360deg); }
    }
    @keyframes progress {
        0% { transform: translateX(-100%); }
        100% { transform: translateX(200%); }
    }
</style>
```