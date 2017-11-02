# PERTEMUAN 16
# Nur Arif

## SCSS

- variabel : bisa memamanggil style menggunkan nama variabel yang di buat

- nesting : di dalam css ada css lagi, maksudnya kita tidak perlu menulisa semua class nya 

    ex : 
    ```scss
    #main-nav {
        logo {
            height: 300px;

            span {
                color: warna;
            }
        }
    }
    ```

    output : 
    
    ```css
    #main-nav .log {
        height: 300px;
    }

    #main-nav .logo span {
        color: white;
    }

    ```

- partials & import : memindahkan file 

- mixins : seperti function bisa memmangiilnya dengan include 

    ex : 

    ```scss
    @mixin border-radius($radius) {
    -webkit-border-radius: $radius;
        -moz-border-radius: $radius;
        -ms-border-radius: $radius;
            border-radius: $radius;
    }

    .box { @include border-radius(10px); }

    ```

    output : 

    ```css 
        .box {
        -webkit-border-radius: 10px;
        -moz-border-radius: 10px;
        -ms-border-radius: 10px;
        border-radius: 10px;
        }
    ```

- extend : penmbahan koma untuk membuat style yang banyak 
    
    ex : 

    ```scss
        .message {
        border: 1px solid #ccc;
        padding: 10px;
        color: #333;
        }

        .success {
        @extend .message;
        border-color: green;
        }

        .error {
        @extend .message;
        border-color: red;
        }

        .warning {
        @extend .message;
        border-color: yellow;
        }
    ```

    output : 
    ```css
    .message, .success, .error, .warning {
    border: 1px solid #cccccc;
    padding: 10px;
    color: #333;
    }

    .success {
    border-color: green;
    }

    .error {
    border-color: red;
    }

    .warning {
    border-color: yellow;
    }
    Operat
    ```

- Operators : bisa melaukakn matematika ( `+, -, *, /, and %` )
    - bisa melakukan penguraan dengan satuan `px`

    ex = 

    ```scss

    .container { width: 100%; }


    article[role="main"] {
    float: left;
    width: 600px / 960px * 100%;
    }

    aside[role="complementary"] {
    float: right;
    width: 300px / 960px * 100%;
    }

    ```

    ```css

        .container {
        width: 100%;
        }

        article[role="main"] {
        float: left;
        width: 62.5%;
        }

        aside[role="complementary"] {
        float: right;
        width: 31.25%;
        }

    ```
