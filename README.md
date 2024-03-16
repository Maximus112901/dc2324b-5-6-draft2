# Assignment 3: Wonkier Button

Create a `WonkierButton.svelte` component and a `Container.svelte` component that have the following behaviors:

1. The `wonkier-button` must have the same behavior as the `WonkyButton` from Assignment 1:
    - The text inside the `wonkier-button` must always depend on the latest `value`.
    - The `value` must have a default value of `0`.
    - If the `value` is divisible by 3, the text must be `Fizz {value}`.
    - If the `value` is divisible by 5, the text must be `Buzz {value}`.
    - If the `value` is divisible by 3 and 5, the text must be `FizzBuzz {value}`.
    - Otherwise, the text must be `{value}`.
    - Whenever the button is clicked, the `value` is incremented by a random integer from `[0,10)`.
1. The `wonkier-button`'s class and text are dependent on each other.
    - Whenever the `wonkier-button` is clicked, the `value` changes, which should change its text, and therefore, its class. 
    - The `wonkier-button`'s class and text can also be changed by typing `Fizz`, `Buzz`, or `FizzBuzz` in the `contenteditable` `div`.
    - For example, when the text on the `wonkier-button` is `Fizz 3`, typing `Buzz` on the `div` will change the `wonkier-button`'s text to `Buzz 3` and its class to `Buzz`.
1. Clicking the `lock-button` will change the `wonkier-button`'s class to `locked` and will prevent any changes to the `wonkier-button`'s class.
    - The `lock-button` must not affect the `wonkier-button`'s text.
    - Clicking the `lock-button` again will "unlock" the `wonkier-button` and allow changes to the `wonkier-button`'s class. 
1. The `WonkierButton.svelte` component will render `<p>FizzBuzz!</p>` inside the `<Container>` when the `wonkier-button`'s text starts with `FizzBuzz`.
    - Modify the `Container.svelte` component such that the `<Container>` can have 4 children when the `wonkier-button`'s text starts with `FizzBuzz`.
    - Otherwise, the `<Container>` should only have 3 children. 
   
> [!IMPORTANT]
> Please only edit the `src/routes/WonkierButton.svelte` and `src/routes/Container.svelte` files.
