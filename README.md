# Go-QRCode

Cross browser QRCode generator for pure javascript. Supported setting for Logo, Background images, etc.

![Preview](assets/qr-code-common.png)

#### REACTJS QR Code Examples,

[Live Demo](https://codesandbox.io/embed/go-qrcode-reactjs-dme8g?fontsize=14&hidenavigation=1&theme=dark "ReactJs QR Code")

```
    import React, { useEffect } from "react";
    import GoQrcode from "go-qrcode";

    const options = {
        text: "https://github.com/RGKrish183/QRCode",
        width: 180,
        height: 180,
        colorDark: "#473C8B",
        colorLight: "#FFFACD",
        logo: "./author-logo.jpg",
        logoWidth: "80",
        logoHeight: "80",
        logoBackgroundColor: "#00b9f5",
        correctLevel: GoQrcode.CorrectLevel.H, // L, M, Q, H
        version: 5
    };

    export default function App() {
        useEffect(() => {
            let domel = document.getElementById("goqrcode");
            new GoQrcode(domel, options);
        }, []);

        return (
            <>
            <div id="goqrcode" />
            </>
        );
    }
```

#### VUEJS QR Code Examples,

[Live Demo](https://codesandbox.io/embed/go-qrcode-vuejs-gccre?fontsize=14&hidenavigation=1&theme=dark "VueJs QR Code")

```
    <template>
    <div>
        <div id="goqrcode"></div>
    </div>
    </template>

    <script>
    import GoQrcode from "go-qrcode";

    export default {
        name: "QRCode",
        mounted() {
            // Options
            let options = {
                text: "https://github.com/RGKrish183/QRCode",
                width: 180,
                height: 180,
                colorDark: "#473C8B",
                colorLight: "#FFFACD",
                logo: "./author-logo.jpg",
                logoWidth: "80",
                logoHeight: "80",
                logoBackgroundColor: "#00b9f5",
                correctLevel: GoQrcode.CorrectLevel.H, // L, M, Q, H
                version: 5
            };

            let domel = document.getElementById("goqrcode");

            // Create new QRCode Object
            new GoQrcode(domel, options);
        }
    };
    </script>
```

#### ANGULAR QR Code Examples,

[Live Demo](https://codesandbox.io/embed/go-qrcode-angular-ji47y?fontsize=14&hidenavigation=1&theme=dark "Angular QR Code")

```
    // .html
    <div id="goqrcode"></div>

    // .ts
    import { Component } from "@angular/core";
    import * as GoQrcode from "go-qrcode";

    @Component({
        selector: "app-root",
        templateUrl: "./app.component.html",
        styleUrls: ["./app.component.css"]
    })
    export class AppComponent {
        title = "CodeSandbox";

        ngAfterContentInit() {
            let options = {
                text: "https://github.com/RGKrish183/QRCode",
                width: 180,
                height: 180,
                colorDark: "#473C8B",
                colorLight: "#FFFACD",
                logo: "../assets/author-logo.jpg",
                logoWidth: "80",
                logoHeight: "80",
                logoBackgroundColor: "#00b9f5",
                correctLevel: GoQrcode.CorrectLevel.H, // L, M, Q, H
                version: 5
            };

            let domel = document.getElementById("goqrcode");

            // Create new QRCode Object
            new GoQrcode(domel, options);
        }
    }

```
