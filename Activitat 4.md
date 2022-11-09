# Activitat 4 - 5 IDEs de Java més utilitzats

## Javier Mouriño Rodríguez

**Eclipse**

Aquesta IDE està disponible per a Windows, Linux i Mac).

Per a instalar Eclipse primer necessitarem tenir el Java. Amb aquest instal·lat, descarreguem el arxiu zip de la versió que vulguem a la seva pagina oficial
i el guardarem a la nostra carpeta personal. després el descomprimirem amb click dret i ens creara una carpeta anomenada Eclipse. Acte seguit mourem aquesta
carpeta al directori opt amb la comanda:

sudo mv eclipse/ /opt/eclipse/

Finalment crearem un accés directe creant el seu arxiu .desktop amb la següent comanda:

sudo nano /usr/share/application/eclipse.desktop

I dins seu introduirem el següent:

[Desktop Entry]
Name=Eclipse IDE
Comment=Eclipse IDE
Exec=/opt/eclipse/eclipse
Icon=/opt/eclipse/icon.xpm
Type=Application
StartupNotify=true
Categories=Utility;Development;IDE;

I ja podrem fer-lo servir.

