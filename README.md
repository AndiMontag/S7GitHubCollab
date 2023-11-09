# Types of Puzzle Games
## By: Andi Montag
### For SDEV 2110
The webpage was designed using different languages, such as: 
* HTML
* CSS
* JavaScript

The webpage provides you the **history** and *creation* of five popular written games. 

To veiw what is in the rep, you can go to [this webpage](https://github.com/AndiMontag/S7GitHubCollab).

For users, when the webpage loads, they will be presented with tabs that have the brief description, history, and photo example of the puzzle that is being discussed, like this... ![Sudoku Image Example](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e0/Sudoku_Puzzle_by_L2G-20050714_standardized_layout.svg/1200px-Sudoku_Puzzle_by_L2G-20050714_standardized_layout.svg.png)

The page primarily shows knowledge of how to utilize tabbed content on a webpage through the use of JavaScript, as shown in the code 
```js
//dropdown divs
class Dropdown {
    constructor(container) {
        this.container = container;
        this.trigger = container.querySelector('.trigger');
        this.content = container.querySelector('.content');
    }
    init(){
        this.trigger.addEventListener('click', () => {
            this.trigger.classList.toggle('active');
            this.content.classList.toggle('active');
        })
    }
}
//create dropdowns
const dropdowns = document.querySelectorAll('.dropdown');
dropdowns.forEach(dropdown => {
    const instance = new Dropdown(dropdown);
    instance.init();
})
```
