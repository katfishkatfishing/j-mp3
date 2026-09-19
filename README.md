# J-mp3

<h2>Portable Music Player</h2>

<p align="center">
  <a href="https://github.com/user-attachments/assets/c255b1d1-a01b-46f7-a71f-36368470523b">
    <img
      src="https://github.com/user-attachments/assets/c255b1d1-a01b-46f7-a71f-36368470523b"
      alt="J-mp3 Portable Music Player"
      width="450"
    />
  </a>
</p>
      <p>Journey of making my own portable music player!</p>
      <p>I got interested in making my own electronics stuff. I'm on a quest to fill my room with cool and useful engineering machines. The first step to any great machine is the electronic components inside it. I'm very new to this, so I'm starting off simple.</p>
      <p>A portable music player inspired by classic iPods, playing audio directly from an inserted microSD card with support for both high-fidelity analog 3.5mm output and Bluetooth audio streaming.</p>
      <p> ⚡Powered by <strong>ESP32-S3</strong> and the PCB dimensions are 📏<strong>60.0*84.3mm</strong> (width*height) 👍</p>
      <p><strong><ins>🚨Note🚨:</ins></strong> I prefer assembling myself so all the PCBs I make <strong><ins>🔴REQUIRE YOU TO SOLDER COMPONENTS YOURSELF🔴</ins></strong>.</p>
      <p>More projects and revisions coming soon🙌!</p>

## Capabilities
### Microcontroller & Audio
- **ESP32-S3** (Dual-core Xtensa® 32-bit LX7, up to 240MHz, 2.4 GHz Wi-Fi & Bluetooth 5 (LE))
- **PCM5102A** Audio Stereo DAC (32-bit, 384kHz high-resolution audio)
- **TDA1308** Class-AB stereo headphone driver amplifier
- **PJ-320B** 3.5mm headphone jack with analog output & Bluetooth audio support

### Display, Controls & Storage
- **1.73" AMOLED Display** (466×466 resolution via high-speed QSPI)
- **EC11E Rotary Encoder** with integrated push button for iPod-like scroll navigation
- Push buttons for power and playback control
- **MicroSD Card Socket** (Hirose DM3AT push-push) for onboard music storage

### Power & Battery Management
- **TP4056** Li-Ion battery charging IC with thermistor temperature sensing
- **DW01A + FS8205A** integrated battery protection (overcharge, overdischarge, overcurrent)
- **TPS2121** Power Multiplexer / Ideal Diode Controller (seamless automatic switching between USB-C and battery)
- **TPS61023** Synchronous boost converter & low-noise **RT9080-33** LDO regulators
- Supports 3.7V LiPo battery (e.g. 755060 3000mAh)
- USB Type-C receptacle for charging and power input

## J-mp3 PCB
### Schematic
<img width="1407" height="632" alt="J-mp3 Schematic 1" src="https://github.com/user-attachments/assets/593c9a7a-ace8-43a7-b47d-b2974178a7af" />

<img width="1635" height="763" alt="J-mp3 Schematic 2" src="https://github.com/user-attachments/assets/30ee4233-5f8a-4cc1-b2d7-ba1b08f5491c" />

<img width="704" height="717" alt="J-mp3 Schematic 3" src="https://github.com/user-attachments/assets/b2bb8e9e-c214-4366-9e0d-1d658a791059" />

<img width="712" height="436" alt="J-mp3 Schematic 4" src="https://github.com/user-attachments/assets/7c3135c2-92d3-4d90-9a4b-3ae96e5c3e89" />

## BOM

| Item | Parts | Qty. | Unit price (USD) | Price per lot (USD) | Source |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Audio jack female | PJ-320B | 1 | 3.2700 | 3.27 | https://www.aliexpress.com/item/1005010463642476.html?spm=a2g0o.productlist.main.1.60817974ZmbdiL&algo_pvid=3c162c60-ca97-44d8-a4ea-9733957078ac&pdp_ext_f=%7B%22order%22%3A%22106%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005010463642476%7C_p_origin_prod%3A |
| Dual N-channel MOSFET | FS8205A | 1 | 1.5900 | 1.59 | https://www.aliexpress.com/item/1005006375737459.html?spm=a2g0o.productlist.main.1.a0b04c51uTVtAf&algo_pvid=7da07ac5-ba7f-498b-ae78-000138901bd1&pdp_ext_f=%7B%22order%22%3A%22244%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005006375737459%7C_p_origin_prod%3A |
| Ideal Diode Controller | TPS2121RUXR | 1 | 2.0900 | 2.09 | https://www.aliexpress.com/item/1005010183114644.html?spm=a2g0o.productlist.main.1.3b79VBZzVBZzNw&algo_pvid=9486a3c5-64df-4774-9556-4dae7f705c93&pdp_ext_f=%7B%22order%22%3A%2224%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005010183114644%7C_p_origin_prod%3A |
| ESP32 MCU unit | ESP32-S31-WROOM-3 | 1 | 5.0000 | 5.00 | https://www.aliexpress.com/item/1005012434557649.html?invitationCode=aWNUM0JlQUVtMVZjRFJ2NUUzd2xwOVE1RklZQWlQWWxPTmxjTXVvbi9hV2VQemFTZUJrNWVWT0s1MU1hdTAyWg&srcSns=sns_Copy&spreadType=socialShare&social_params=6000474898907&bizType=ProductDetail&spreadCode=aWNUM0JlQUVtMVZjRFJ2NUUzd2xwOVE1RklZQWlQWWxPTmxjTXVvbi9hV2VQemFTZUJrNWVWT0s1MU1hdTAyWg&aff_fcid=838605f6547d4cdc84d85aee383cff12-1789809629059-02194-_c4m7gKM3&tt=MG&aff_fsk=_c4m7gKM3&aff_platform=default&sk=_c4m7gKM3&aff_trace_key=838605f6547d4cdc84d85aee383cff12-1789809629059-02194-_c4m7gKM3&shareId=6000474898907&businessType=ProductDetail&platform=AE&terminal_id=1d9dfb3eef574216a2bcb273506f9cd3&afSmartRedirect=y |
| Boost Voltage Converter | TPS61023DRLR | 1 | 0.1800 | 0.18 | https://www.aliexpress.com/item/1005008589999406.html?spm=a2g0o.productlist.main.1.7ed1dAWodAWo0a&algo_pvid=7237dc5c-62cd-42a2-a2e9-dc6ba816f7c3&pdp_ext_f=%7B%22order%22%3A%22302%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005008589999406%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 1uF 0402 | 8 | 0.2550 | 2.04 | https://www.aliexpress.com/item/1005012364450156.html?spm=a2g0o.productlist.main.1.589f1Ml51Ml5PA&algo_pvid=64ebbb0e-c998-4523-81f0-ca4e95cd79e7&pdp_ext_f=%7B%22order%22%3A%221484%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005012364450156%7C_p_origin_prod%3A |
| P-Channel MOSFET | AO3401A | 1 | 1.9900 | 1.99 | https://www.aliexpress.com/item/1005008388291353.html?spm=a2g0o.productlist.main.1.25206b4c4LUtde&algo_pvid=8b50fb0f-e682-4ae7-85c1-8edc45618de3&pdp_ext_f=%7B%22order%22%3A%22692%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005008388291353%7C_p_origin_prod%3A |
| Diode | 1N4148 | 2 | 0.9850 | 1.97 | https://www.aliexpress.com/item/1005007160563285.html?spm=a2g0o.productlist.main.5.49757952BcmT3Y&algo_pvid=de4616c8-ec89-4be4-9121-617d58f16258&pdp_ext_f=%7B%22order%22%3A%222068%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007160563285%7C_p_origin_prod%3A |
| Audio Stereo DAC | PCM5102A | 1 | 4.4600 | 4.46 | https://www.aliexpress.com/item/1005006267865363.html?spm=a2g0o.detail.pcDetailTopMoreOtherSeller.5.308ezYUgzYUgEv&gps-id=pcDetailTopMoreOtherSeller&scm=1007.40050.354490.0&scm_id=1007.40050.354490.0&scm-url=1007.40050.354490.0&pvid=3709ad84-1f45-4f2f-a9d4-9019da4e1276&_t=gps-id%3ApcDetailTopMoreOtherSeller%2Cscm-url%3A1007.40050.354490.0%2Cpvid%3A3709ad84-1f45-4f2f-a9d4-9019da4e1276%2Ctpp_buckets%3A668%232846%238116%232002&pdp_ext_f=%7B%22order%22%3A%2250%22%2C%22eval%22%3A%221%22%2C%22sceneId%22%3A%2230050%22%2C%22fromPage%22%3A%22recommend%22%7D&utparam-url=scene%3ApcDetailTopMoreOtherSeller%7Cquery_from%3A%7Cx_object_id%3A1005006267865363%7C_p_origin_prod%3A |
| Headphone Driver Amplifier | TDA1308 | 1 | 2.0800 | 2.08 | https://www.aliexpress.com/item/33051574290.html?spm=a2g0o.productlist.main.16.cf5d7988hDu7CF&algo_pvid=2a75b342-aa82-4fe0-941c-90eca8f2c625&pdp_ext_f=%7B%22order%22%3A%2213%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A33051574290%7C_p_origin_prod%3A |
| Bipolar transistor symbol | NPN SOT-23 | 1 | 5.1200 | 5.12 | https://www.aliexpress.com/item/1005012628572946.html?spm=a2g0o.productlist.main.1.1d04e8O1e8O1UQ&algo_pvid=8a51f11c-8b8d-4c0b-af60-1e4180ac1a48&pdp_ext_f=%7B%22order%22%3A%2229%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005012628572946%7C_p_origin_prod%3A |
| Generic connector, 02x12 | Conn_02x12_Counter_Clockwise | 1 | 1.5000 | 1.50 | https://www.aliexpress.com/item/1005007611939409.html |
| Generic connector, 01x04 | Conn_01x04_Pin | 1 | 1.1700 | 1.17 | https://www.aliexpress.com/item/1005012793102722.html?spm=a2g0o.productlist.main.12.573ed4KHd4KHjM&aem_p4p_detail=202609190328541006253439417720000081299&algo_pvid=80c6bcb6-eae0-4a64-9e2c-b5b2595232e3&pdp_ext_f=%7B%22order%22%3A%226%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005012793102722%7C_p_origin_prod%3A&search_p4p_id=202609190328541006253439417720000081299_3 |
| Inductor SMD | 2.2uH 0603 | 1 | 2.1400 | 2.14 | https://www.aliexpress.com/item/1005004840798951.html?spm=a2g0o.productlist.main.1.4afbESaQESaQvr&algo_pvid=e6f9ad16-910b-43de-9ffc-c876db7ab0df&pdp_ext_f=%7B%22order%22%3A%22359%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005004840798951%7C_p_origin_prod%3A |
| Linear Voltage Regulator | RT9080-33GJ5 | 2 | 0.7650 | 1.53 | https://www.aliexpress.com/item/1005004159688937.html?spm=a2g0o.productlist.main.1.51784d72rSYVqB&algo_pvid=080971bf-6546-4391-82a5-f72f196448dc&pdp_ext_f=%7B%22order%22%3A%2266%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005004159688937%7C_p_origin_prod%3A |
| Micro SD Card Socket | Hirose DM3AT-SF-PEJM5 | 1 | 1.2000 | 1.20 | https://www.aliexpress.com/item/1005008529231123.html?spm=a2g0o.productlist.main.15.780faIWTaIWTP1&algo_pvid=3f337965-ee0b-478d-a7b6-a5af69d736c1&pdp_ext_f=%7B%22order%22%3A%2225%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005008529231123%7C_p_origin_prod%3A |
| Battery protection | DW01A | 1 | 2.5400 | 2.54 | https://www.aliexpress.com/item/1005008626342372.html?spm=a2g0o.productlist.main.1.50895bfdtbnlKJ&algo_pvid=237b56ff-402d-4134-ad38-9a508b1e9970&pdp_ext_f=%7B%22order%22%3A%2270%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005008626342372%7C_p_origin_prod%3A |
| Capacitor Tantalum SMD | 100uF 3528-12 (Metric) | 1 | 4.0500 | 4.05 | https://my.mouser.com/en/ProductDetail/Vishay-Sprague/293D107X9004B2TE3?qs=N31o%252Bt096guiYtrI%2FhDC5g%3D%3D |
| Capacitor Tantalum SMD | 10uF 0603 | 4 | 2.4200 | 9.68 | https://www.aliexpress.com/item/1005003344584575.html?spm=a2g0o.productlist.main.1.7884v2Zuv2ZurL&algo_pvid=d34dac6c-7fb3-48c0-9352-0cc876b7f408&pdp_ext_f=%7B%22order%22%3A%2242%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005003344584575%7C_p_origin_prod%3A |
| Push button switch | SW-SMD_TC-1101V-C-B-W | 1 | 0.4000 | 0.40 | https://item.szlcsc.com/300030.html |
| Push button switch SMD | SW_SPST_B3U-1000P | 2 | 0.7300 | 1.46 | https://www.aliexpress.com/item/1005009548875400.html?spm=a2g0o.productlist.main.1.56ebP1y3P1y3Yd&algo_pvid=e205a10a-479c-4a7d-81eb-9951e2930e82&pdp_ext_f=%7B%22order%22%3A%223%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005009548875400%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 10k 0805 | 13 | 0.1531 | 1.99 | https://www.aliexpress.com/item/1005007183002569.html?spm=a2g0o.productlist.main.1.68b66b95isN6aN&algo_pvid=385a7354-aa7a-4e7f-8ef9-8c0311d953be&pdp_ext_f=%7B%22order%22%3A%2276%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007183002569%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 2k 0603 | 1 | 1.8000 | 1.80 | https://www.aliexpress.com/item/1005003529112557.html?spm=a2g0o.productlist.main.7.4aee65557cxcrB&algo_pvid=0d3dc69f-c884-4762-8069-30f583ccfdb1&pdp_ext_f=%7B%22order%22%3A%22476%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005003529112557%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 82k 0805 | 1 | 2.0300 | 2.03 | https://www.aliexpress.com/item/1005007183002569.html?spm=a2g0o.productlist.main.1.68b66b95isN6aN&algo_pvid=385a7354-aa7a-4e7f-8ef9-8c0311d953be&pdp_ext_f=%7B%22order%22%3A%2276%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007183002569%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 100 0402 | 1 | 1.3800 | 1.38 | https://www.aliexpress.com/item/1005003721873929.html?spm=a2g0o.productlist.main.1.29821u3H1u3HkD&algo_pvid=0c4eed70-6ca0-4e08-b34a-7ee8ebfe2859&pdp_ext_f=%7B%22order%22%3A%22285%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005003721873929%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 3.9k 0402 | 4 | 0.3450 | 1.38 | https://www.aliexpress.com/item/1005003721873929.html?spm=a2g0o.productlist.main.1.29821u3H1u3HkD&algo_pvid=0c4eed70-6ca0-4e08-b34a-7ee8ebfe2859&pdp_ext_f=%7B%22order%22%3A%22285%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005003721873929%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 1m 0603 | 1 | 1.4800 | 1.48 | https://www.aliexpress.com/item/1005010109041806.html?spm=a2g0o.productlist.main.1.4a12d8mrd8mrat&algo_pvid=af229fc5-fa32-4342-b395-68c0d5cc9c78&pdp_ext_f=%7B%22order%22%3A%22328%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005010109041806%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 5k1 0603 | 2 | 0.8750 | 1.75 | https://www.aliexpress.com/item/1005003529112557.html?spm=a2g0o.productlist.main.7.4aee65557cxcrB&algo_pvid=0d3dc69f-c884-4762-8069-30f583ccfdb1&pdp_ext_f=%7B%22order%22%3A%22476%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005003529112557%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 1k 0402 | 1 | 1.3800 | 1.38 | https://www.aliexpress.com/item/1005003721873929.html?spm=a2g0o.productlist.main.1.29821u3H1u3HkD&algo_pvid=0c4eed70-6ca0-4e08-b34a-7ee8ebfe2859&pdp_ext_f=%7B%22order%22%3A%22285%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005003721873929%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 100k 0805 | 6 | 0.3333 | 2.00 | https://www.aliexpress.com/item/1005007183002569.html?spm=a2g0o.productlist.main.1.68b66b95isN6aN&algo_pvid=385a7354-aa7a-4e7f-8ef9-8c0311d953be&pdp_ext_f=%7B%22order%22%3A%2276%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007183002569%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 4.7k 0805 | 1 | 2.0000 | 2.00 | https://www.aliexpress.com/item/1005007183002569.html?spm=a2g0o.productlist.main.1.68b66b95isN6aN&algo_pvid=385a7354-aa7a-4e7f-8ef9-8c0311d953be&pdp_ext_f=%7B%22order%22%3A%2276%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007183002569%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 470 0603 | 2 | 0.9000 | 1.80 | https://www.aliexpress.com/item/1005003529112557.html?spm=a2g0o.productlist.main.7.4aee65557cxcrB&algo_pvid=0d3dc69f-c884-4762-8069-30f583ccfdb1&pdp_ext_f=%7B%22order%22%3A%22476%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005003529112557%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 43k 0805 | 1 | 2.0300 | 2.03 | https://www.aliexpress.com/item/1005007183002569.html?spm=a2g0o.productlist.main.1.68b66b95isN6aN&algo_pvid=385a7354-aa7a-4e7f-8ef9-8c0311d953be&pdp_ext_f=%7B%22order%22%3A%2276%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007183002569%7C_p_origin_prod%3A |
| Ceramic resistor SMD | 732k 0603 | 1 | 2.1000 | 2.10 | https://www.aliexpress.com/item/1005005459557840.html?spm=a2g0o.productlist.main.1.552eKaoZKaoZOW&algo_pvid=d5c5bb48-d381-4227-ba1e-46e8d7582c70&pdp_ext_f=%7B%22order%22%3A%2277%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005005459557840%7C_p_origin_prod%3A |
| Rotary encoder with switch | EC11E | 1 | 2.9400 | 2.94 | https://www.aliexpress.com/item/32976046900.html?spm=a2g0o.detail.pcDetailBottomMoreOtherSeller.13.6474lV6ElV6Evn&gps-id=pcDetailBottomMoreOtherSeller&scm=1007.14452.396806.0&scm_id=1007.14452.396806.0&scm-url=1007.14452.396806.0&pvid=aeb64c1f-7a29-4ad5-933b-e98472c40c59&_t=gps-id%3ApcDetailBottomMoreOtherSeller%2Cscm-url%3A1007.14452.396806.0%2Cpvid%3Aaeb64c1f-7a29-4ad5-933b-e98472c40c59%2Ctpp_buckets%3A668%232846%238116%232002&pdp_ext_f=%7B%22order%22%3A%22547%22%2C%22eval%22%3A%221%22%2C%22sceneId%22%3A%2230050%22%2C%22fromPage%22%3A%22recommend%22%7D&utparam-url=scene%3ApcDetailBottomMoreOtherSeller%7Cquery_from%3A%7Cx_object_id%3A32976046900%7C_p_origin_prod%3A&search_p4p_id=202608180535232983463426697065023539_2 |
| Single-cell battery | 755060 LiPo 3000mAh | 1 | 8.9000 | 8.90 | https://www.aliexpress.com/item/1005006259194674.html?spm=a2g0o.productlist.main.2.36fb5dcS5dcSS8&algo_pvid=e5418aaa-c7d1-42cf-949d-d8510645f5cd&pdp_ext_f=%7B%22order%22%3A%22151%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005006259194674%7C_p_origin_prod%3A |
| Li-lon Battery Charger | TP4056 | 1 | 0.5200 | 0.52 | https://www.aliexpress.com/item/1005005487915175.html?spm=a2g0o.productlist.main.8.4b6058c9uwNrRB&aem_p4p_detail=202609190258166749914128201200000080084&algo_pvid=0f66a318-1b84-45cd-80d0-95d22f5eb897&pdp_ext_f=%7B%22order%22%3A%22255%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005005487915175%7C_p_origin_prod%3A&search_p4p_id=202609190258166749914128201200000080084_2 |
| Thermistor | 10k 0402 | 1 | 2.8100 | 2.81 | https://www.aliexpress.com/item/1005010466857933.html?spm=a2g0o.productlist.main.2.4fb8w7gbw7gbc4&algo_pvid=0c2c7f04-0061-4f44-94c4-1ea901b197c0&pdp_ext_f=%7B%22order%22%3A%2228%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005010466857933%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 100nF 0603 | 4 | 0.5025 | 2.01 | https://www.aliexpress.com/item/1005007660078779.html?spm=a2g0o.productlist.main.1.41ad17afXggjid&algo_pvid=94b82144-0913-4272-a928-8d27b54f2344&pdp_ext_f=%7B%22order%22%3A%22790%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007660078779%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 10uF 0805 | 5 | 0.5280 | 2.64 | https://www.aliexpress.com/item/1005012364450156.html?spm=a2g0o.productlist.main.1.4a92101aYp6fpR&algo_pvid=def9331d-468c-46b6-a7c2-2492d88f5a7b&pdp_ext_f=%7B%22order%22%3A%221484%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005012364450156%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 1uF 0805 | 3 | 0.7833 | 2.35 | https://www.aliexpress.com/item/1005012364450156.html?spm=a2g0o.productlist.main.1.4a92101aYp6fpR&algo_pvid=def9331d-468c-46b6-a7c2-2492d88f5a7b&pdp_ext_f=%7B%22order%22%3A%221484%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005012364450156%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 10nF 0603 | 1 | 2.0000 | 2.00 | https://www.aliexpress.com/item/1005007660078779.html?spm=a2g0o.productlist.main.1.41ad17afXggjid&algo_pvid=94b82144-0913-4272-a928-8d27b54f2344&pdp_ext_f=%7B%22order%22%3A%22790%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007660078779%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 22uF 0805 | 3 | 1.1833 | 3.55 | https://www.aliexpress.com/item/1005012364450156.html?spm=a2g0o.productlist.main.1.4a92101aYp6fpR&algo_pvid=def9331d-468c-46b6-a7c2-2492d88f5a7b&pdp_ext_f=%7B%22order%22%3A%221484%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005012364450156%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 0.1uF 0805 | 2 | 0.7150 | 1.43 | https://www.aliexpress.com/item/1005006142309480.html?spm=a2g0o.productlist.main.2.5b5d23fbK7Es7i&algo_pvid=b69da919-24fd-4e5c-b25c-abccb2827b6a&pdp_ext_f=%7B%22order%22%3A%226337%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005006142309480%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 100uF 0805 | 2 | 6.8600 | 13.72 | https://www.aliexpress.com/item/1005005590636993.html?spm=a2g0o.productlist.main.2.258950300kp4f9&algo_pvid=b9072869-1443-4f9f-9d83-403e7e57091f&pdp_ext_f=%7B%22order%22%3A%22357%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005005590636993%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 0.1uF 0201 | 4 | 0.2375 | 0.95 | https://www.aliexpress.com/item/1005008499718166.html?spm=a2g0o.productlist.main.3.4f072457BLp6JC&algo_pvid=708b6ba6-6d07-40b3-8c9c-719163e04cda&pdp_ext_f=%7B%22order%22%3A%22397%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005008499718166%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 2.2uF 0603 | 2 | 1.0150 | 2.03 | https://www.aliexpress.com/item/1005007660078779.html?spm=a2g0o.productlist.main.1.41ad17afXggjid&algo_pvid=94b82144-0913-4272-a928-8d27b54f2344&pdp_ext_f=%7B%22order%22%3A%22790%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007660078779%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 1nF 0603 | 1 | 1.9800 | 1.98 | https://www.aliexpress.com/item/1005007660078779.html?spm=a2g0o.productlist.main.1.41ad17afXggjid&algo_pvid=94b82144-0913-4272-a928-8d27b54f2344&pdp_ext_f=%7B%22order%22%3A%22790%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007660078779%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 2.2nF 0805 | 2 | 1.5200 | 3.04 | https://www.aliexpress.com/item/33039604868.html?spm=a2g0o.productlist.main.10.3afdzjnrzjnr3Q&algo_pvid=66e61c7f-f79e-40bc-bf5d-0d52052e1876&pdp_ext_f=%7B%22order%22%3A%2258%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A33039604868%7C_p_origin_prod%3A |
| Ceramic capacitor SMD | 100pF 0603 | 1 | 2.0300 | 2.03 | https://www.aliexpress.com/item/1005007660078779.html?spm=a2g0o.productlist.main.1.1729LAMPLAMPww&algo_pvid=134453e7-f153-4dc4-9327-eebe4236be4f&pdp_ext_f=%7B%22order%22%3A%22790%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007660078779%7C_p_origin_prod%3A |
| USBType-C Receptacle | USB4125-GF-A | 1 | 0.6000 | 0.60 | https://www.digikey.my/en/products/detail/gct/USB4125-GF-A/13547388 |
| AMOLED Display | 1.73 inch 466x466 QSPI | 1 | 7.4700 | 7.47 | https://item.taobao.com/item.htm?id=952177467095&mi_id=0000jOy7u6r5ZkyFyRkc3t68ZxdEMGvtNs0QXCuW6-oULvo&spm=a21xtw.29178619.0.0&xxc=shop |
| Total+Shipping+Tax | - | - | - | 139.55± | - |

### Footprint
<table>
  <tr>
    <td>
      <img width="360" height="430" alt="J-mp3 Footprint Front" src="https://github.com/user-attachments/assets/84b32400-c673-4837-bc9d-269db9f22249" />
    </td>
    <td>
      <img width="360" height="430" alt="J-mp3 Footprint Back" src="https://github.com/user-attachments/assets/ff473c9a-f2d8-4145-8b66-646518425d75" />
    </td>
  </tr>
  <tr>
    <td>
      <img width="360" height="430" alt="J-mp3 Inner Layer 1" src="https://github.com/user-attachments/assets/5888a543-b334-4aa7-855b-4935c94e0aa1" />
    </td>
    <td>
      <img width="360" height="430" alt="J-mp3 Inner Layer 2" src="https://github.com/user-attachments/assets/c4c27749-a432-4141-953e-bc77c2d40104" />
    </td>
  </tr>
</table>

### 3D View
<table>
  <tr>
    <td>
      <img width="400" alt="J-mp3 3D Front" src="https://github.com/user-attachments/assets/c255b1d1-a01b-46f7-a71f-36368470523b" />
    </td>
    <td>
      <img width="400" alt="J-mp3 3D Back" src="https://github.com/user-attachments/assets/2141cb95-9680-4c3a-9d35-e3b9ce12d729" />
    </td>
  </tr>
</table>
