# melipilla-iot-apr-11grupo
En la agricultura, los invernaderos permiten controlar las condiciones climáticas para optimizar la producción de cultivos. Sin embargo, muchos pequeños productores carecen de sistemas automatizados y deben realizar ajustes manuales. Este proyecto busca implementar un invernadero inteligente en maqueta utilizando IoT y Raspberry Pi, con capacidad de medir variables ambientales y controlar ventilación e iluminación automáticamente.
Objetivo General: Diseñar y prototipar un invernadero inteligente de bajo costo que controle temperatura, humedad y luz de manera automática.


Integrantes: Alexander Meza - Matias Aliaga


---

## 🔧 Dispositivos y materiales

### 1. **Controlador principal**

* **Raspberry Pi (3B+, 4 o Zero 2 W)** → será el cerebro del sistema.
* **MicroSD (16-32 GB)** → para sistema operativo y programas.
* **Fuente de poder (5V 2-3A)** → estable para Raspberry Pi.

---

### 2. **Sensores**

* **DHT22 o DHT11** → mide temperatura y humedad del aire.
* **BH1750 o LDR (fotoresistor)** → mide luminosidad (para controlar LEDs o determinar apertura/cierre de ventilación).


---

### 3. **Actuadores**

* **Módulo de relés de 2 a 4 canales (5V)** → para encender/apagar ventiladores, luces, bomba de agua.
* **Ventilador pequeño (5V o 12V, tipo cooler de PC)** → simula la ventilación del invernadero.
* **Tira LED blanca o lámpara LED (5V/12V)** → para simular luz artificial en caso de baja luminosidad.


---

### 4. **Estructura (maqueta de invernadero)**

* Caja de acrílico, plástico transparente o incluso caja de vidrio/acetato → simulará el invernadero.
* Cableado Dupont macho-hembra.
* Protoboard o placa de pruebas.

---

### 5. **Conectividad y visualización**

* **Node-RED o Grafana** en la Raspberry Pi → dashboard web para controlar y visualizar datos.
* **MQTT (Mosquitto)** → para comunicación interna de los sensores/actuadores.
* Acceso desde celular o PC a la interfaz web.

---

## ⚡ Diagrama funcional básico

1. **Sensores → Raspberry Pi**: capturan datos (temp, humedad, luz).
2. **Raspberry Pi → Relés**: decide cuándo encender ventilador, luces o bomba.
3. **Dashboard web**: permite ver datos en tiempo real y activar manualmente ventilación o luz.

---

## 💡 Ejemplo de uso en tu maqueta

* Si **temperatura > 28°C** → encender ventilador.
* Si **luz < umbral** → encender LED de apoyo.
* Todo visible en un **dashboard accesible desde tu celular**.

---

