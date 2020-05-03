# Go-QRCode

Cross browser QRCode generator for pure javascript. Supported setting for Logo, Background images, etc.

![Basic Preview](assets/qr-code-basic.png)

![Logo Preview](assets/qr-code-with-author-logo.png)

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
