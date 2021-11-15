# Onedark theme for reveal.js

A [reveal.js](https://revealjs.com) theme based on the
[onedark](https://github.com/joshdick/onedark.vim) colorscheme.


## How to use?

1. Clone this repository to your computer:
    ```
    git clone https://github.com/santisoler/onedark-reveal.js
    ```
1. Move to the repo directory:
    ```
    cd onedark-reveal.js
    ```
1. Copy the `onedark.css` file into your `reveal.js` project: and change the theme
    ```
    cp onedark.css <path/to/your/reveal.js>/dist/theme/onedark.css
    ```
1. Finally, replace the theme selection in the `index.html` of your project:
    ```html
    <link rel="stylesheet" href="dist/theme/onedark.css" id="theme" />

    ```

## How to build?

If you want to generate your own `onedark.css` file because you want to modify
it, you can build it from the `onedark.scss` file.

1. Install `sassc` from your package manager.
    * For Debian and Ubuntu:
        ```
        sudo apt install sassc
        ```
    * For Arch and Manjaro:
        ```
        sudo pacman -S sassc
        ```
1. Clone this repository to your computer:
    ```
    git clone https://github.com/santisoler/onedark-reveal.js
    ```
1. Clone the reveal.js repo:
    ```
    git clone https://github.com/hakimel/reveal.js.git
    ```
1. Copy the `onedark.scss` file into the reveal.js folder that contains the
   sources for the themes:
    ```
    cp onedark-reveal.js reveal.js/css/theme/source/
    ```
1. Change directory and build the `onedark.css` file:
    ```
    cd reveal.js/css/theme/source/
    sassc onedark.sassc onedark.css
    ```
1. Once the `onedark.css` file is created, copy to your reveal.js project and
   select it on `index.html` as shown above.
