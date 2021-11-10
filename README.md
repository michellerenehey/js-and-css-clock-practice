# js-and-css-clock-practice
JS 30 - day 2!

# HTML
- div for clock
- child div for clock-face
- grandchildren div: second hand, minute hand, hour-hand

# CSS: 
- make the hands rotate on the right-most side of element (so they are held in the center): transform-origin: 100%; 
- tranform: rotate(90deg) so the hand are pointing up! 
- apply transition so the rotation is smooth; apply transition-timing-function so that the transition of the hands moving looks like a real "bounce-back" clock

# JS: 

- create a setDate() function which grabs the current date and runs on a setInterval timer: setInterval(setDate(), 1000). split up for each hand: 
    - getSeconds
        - set degrees: (seconds / 60) * 360
        - rotate degrees: ((seconds / 60) * 360) + 90
        - grab item from DOM
        - apply styles to the item from the DOM (.style.transform = rotate(secondsDegrees)) and use template literals for the degrees!
    - getMinutes *repeat above*
    - getHours *repeat above*