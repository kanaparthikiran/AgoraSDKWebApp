# OpenDuoLive-Web

This Agora Application that will help get live video broadcasting and chat messaging integrated directly into JS applications using the Agora Video SDK + Signaling SDK.

With this sample app, We can:

- Join broadcast as an broadcasting member
- Join broadcast as an audience member
- Chat with broadcasters and viewers

## Running the App

The Video SDK and Signaling SDK are already included in this demo inside 'src/utils'.

Create a developer account at [Agora.io](https://dashboard.agora.io/signin/), and obtain an App ID. Update "agora.config.js" inside the 'static' folder with your App ID.

```
const AGORA_APP_ID = 'ADD-APP-ID-HERE'
```

Run the following commands

```
npm install
npm audit fix
npm run build
cd dist

// SSL & Deploy to HTTPS
openssl req -newkey rsa:2048 -nodes -keyout key.pem -x509 -days 365 -out certificate.pem
sudo http-server ./ -p 443 --ssl -C certificate.pem -K key.pem
```



## License

The MIT License (MIT).
