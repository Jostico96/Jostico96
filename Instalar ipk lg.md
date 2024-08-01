> Uso ConnectBot con mi teléfono Android para conectarme al televisor a través de SSH (habilita SSH en el canal homebrew) (no necesitas usar Connectbot, cualquier cliente SSH debería funcionar)
> 
> El nombre de host es root@dirección IP del televisor. Por ejemplo, para mí es root@192.168.50.4. La contraseña es alpine.
> 
> Al conectarse, utilice primero esta línea:
> 
> `curl -k -L -o /tmp/app.ipk 'https://github.com/webosbrew/youtube-webos/releases/download/v0.3.3/youtube.leanback.v4_0.3.3_all.ipk' `
> 
> Haga clic en Enter
> 
> y luego esta linea
> 
> `luna-send-pub -w 10000 -i 'luna://com.webos.appInstallService/dev/install' '{"id":"com.ares.defaultName","ipkUrl":"/tmp/app.ipk","subscribe":true}'`
> 
> Haga clic en Enter
> 
> Al menos esos son los pasos que se siguen en mi caso. Uso un OLED C9.

