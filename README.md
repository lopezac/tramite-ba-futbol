# tramite-ba-futbol

Hola, este script lo cree para ahorrar tiempo, para automatizar un tramite que cuando lo tenia que hacer era bastante tedioso.

El script ahora soporta **52 polideportivos** de Buenos Aires y automatiza la reserva de canchas para múltiples deportes:

## Polideportivos Soportados

✅ **52 polideportivos** en total, incluyendo:
- Parque Patricios, Martin Fierro, Don Pepe (originalmente soportados)
- Costa Rica, Santojanni, Avellaneda, Colegiales, Dorrego, Onega, Pereyra, Pomar, Sarmiento (anteriormente no soportados)
- Y 40 polideportivos adicionales cubriendo todos los barrios de Buenos Aires

## Deportes Disponibles

🏆 **Futbol**: 52 polideportivos
- Canchas de Futbol 5, 7, 9 y 11
- Diferentes tipos de superficie (asfalto, sintético, etc.)

🏀 **Basquet**: 8 polideportivos
- Canchas cubiertas y al aire libre

🎾 **Tennis**: 2 polideportivos  
- Canchas de tennis profesionales

## Funcionalidades

El script pregunta al usuario:
- El polideportivo deseado (de una lista de 52 opciones)
- El deporte (futbol, basquet, tennis según disponibilidad)
- El tamaño de cancha (5, 7, 9, 11 según el polideportivo)
- El tipo de cancha (cuando hay opciones)
- La fecha y hora de reserva
- Los datos de la cuenta miBA (email y contraseña)

Automatiza desde abrir el navegador con [Selenium](https://www.selenium.dev/documentation/webdriver/), iniciar sesión, pedir turno, seleccionar horario y fecha, rellenar los datos (nombre, apellido, email y dni) con datos falsos gracias al paquete [Faker](https://github.com/joke2k/faker).

Si tenes errores abriendo el navegador Firefox, y estas en Ubuntu seguramente tengas instalado el navegador con un snap lo que te recomendario seria desintales el navegador y lo instales sin snap.

Aca hay una [guia](https://linuxconfig.org/switching-to-firefoxs-deb-installation-on-ubuntu-22-04-a-guide-to-avoiding-snap-packages) de como desinstalar el Firefox snap e instalarlo como un paquete normal en Ubuntu.

# Instalación

```bash
  # clonamos el repositorio
  git clone https://github.com/lopezac/tramite-ba-futbol.git
  # nos movemos a la carpeta del repositorio clonado
  cd tramite-ba-futbol
  # creamos un python virtual environment
  python3 -m venv .venv
  # entramos al virtual environment
  source .venv/bin/activate
  # instalamos dependencias
  pip3 install -r requirements.txt
  # corremos el programa
  python3 main.py
```
