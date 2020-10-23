# normalize-css

TIL that in order to make browsers render all elements more consistently, and in line with modern standards, you can use the `normalize.css` module in your project.

eg. In your app.js main file, import it:

```
import 'normalize.css/normalize.css'
```

Note: Webpack needs to be able to process the css file. Not sure how this works yet with the create-react-app but here's a snippet of how the webpack.config.js looks like.

```
...
        }, {
            test: /\.s?css$/,
            use: [
                'style-loader',
                'css-loader',
                'sass-loader'
            ]
        }]
    },
...
```

Reference: https://necolas.github.io/normalize.css/