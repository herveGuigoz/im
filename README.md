# im

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


.about-container {
            position: absolute;
            top: 0;
            left: 0;
            z-index: 99;
            width: 100%;
            height: 100%;
            overflow: hidden;
            display: none
        }
.about-container .about-overlay {
            position: absolute;
            top: 0;
            left: 0;
            z-index: 98;
            background: #000;
            opacity: 0;
            width: 100%;
            height: 100%
        }

        @media (min-width:960px) {
            .about-container .about-overlay {
                background: rgba(0, 0, 0, 0)
            }
        }

.about-container .about-wrapper {
            position: absolute;
            bottom: 0;
            right: 0;
            z-index: 99;
            background: #fbfaf7;
            width: 95%;
            height: 88%;
            -webkit-transform: translateY(100%);
            -ms-transform: translateY(100%);
            transform: translateY(100%);
            overflow: scroll;
            -webkit-overflow-scrolling: touch
        }

        @media (min-width:960px) {
            .about-container .about-wrapper {
                overflow: auto;
                -webkit-overflow-scrolling: initial;
                width: 96.09375%;
                height: 91.52941%
            }
        }