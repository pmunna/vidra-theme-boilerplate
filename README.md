# Vidra Webshop theme Design System

Vidra Webshop theme Design System, progettato da Bemind Interactive.

&nbsp;

![screenshot-desktop](https://github.com/vidra-io/Webshop-boilerplate/blob/master/pages/screenshot.png)

&nbsp;

# Development

I temi vengono compilati usando Node.js, dorvete installarlo globalmente prima di poter utilizzare il sistema.  
Dopo aver fatto ciò, andate nella directory del tema ed eseguite il seguente comando:  

```bash
$ npm install
```

Se non si sono verificati problemi, potrete modificare i file delle pagine in `/pages/`, e i file css, js e tali in `/assets/`.  
Nota bene: Il file `/pages/layout.hbs` viene generato in tutte le pagine.  
Potete verificare lo stato del tema con una demo nel vostro browser eseguendo:

```bash
$ npm start
```

Nella demo, tutti i dati visibili, come i nomi dei prodotti, prezzi, collezioni ec. vengono recuperati dai file .json in  `/data/`.  
Ogni pagina è legata a un file .json differente, eccetto always.json che viene visualizzato in qualsiasi pagin.a  
Esempio: in `account.json` verranno visualizzati solo i dati relativi all'account, e in  `cart.json` solo i dati dei prodotti nel carrello.  

Potete esportare il tema eseguendo il comando:  

```bash
$ npm run zip
```

Dopodiché potrete caricare il file zip generato dal comando sulla dashboard Vidra del vostro shop (sotto `Channels` > `Configurazione` del vostro negozio)
e visualizzare il vostro tema sul vostro shop online.

Nota bene: I file json nella cartella `/data/` non hanno alcuna utilità nello shop online, ma solo nella demo.  

I temi utilizzano il sistema [handlebars.js](https://handlebarsjs.com/) troverete una guida alle variabili utilizzabili in `/node_modules/webshop-theme-kit/bin/docs`
e degli esempi standard dei file in `/node_modules/webshop-theme-kit/test/supportfiles`  