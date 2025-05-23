![Image_0](https://github.com/user-attachments/assets/1fd80f67-640a-42f5-bc25-c7b80e06774a)

# Introduction
I wanted to add another level of security to my computer, because, you know, why not? This makes it so that I am the only one who can log into my computer, regardless of who knows my password.

# Material(s)

* [USB C Extension Cable ($7.99)](https://www.amazon.com/gp/product/B0CPM2PT13/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&th=1)

* [Right Angle USB C Adapter ($9.39)](https://www.amazon.com/gp/product/B0BRCNMRVK/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&th=1)

* [YubiKey C Bio - FIDO Edition ($95)](https://www.yubico.com/product/yubikey-bio-series/yubikey-c-bio/)

* [3 x 1 Inch Velcro Strips ($6.97)](https://www.amazon.com/VELCRO-Brand-ALFA-LOK-Fasteners-Multidirectional/dp/B07FYZVBNR/ref=sr_1_1?crid=OA1GB7583ZL8&dib=eyJ2IjoiMSJ9.QieCE0WxvAcxz9y1kZJVAonSFhsY7pBV07Edsze4TQAgv19HyzW9AQnijbX3kDSBHChSj5wyd-_laazS7ziTE6V31vwi6HrKkewwEvF9TB691VEM7EsjF2-kh56PSRqBNzXWNTTb1S55vA9wPhQviG_UQS7MH7AIdVV6F2_r82x9NwfMrYOhyAWOjcnI57xj78qkLTUndU62FY2Q_PLKmTgu-p0ke2fa7OA7viO0nOY.405yZfjst5KSVmS4lAc55yJQCYL-N8JVzgsxM4b1ErA&dib_tag=se&keywords=velcro%2Boutdoor%2Bextreme%2Block&qid=1737911959&sprefix=velcro%2Boutdoor%2Bextreme%2Block%2Caps%2C118&sr=8-1&th=1)

* [10x2mm Magnets ($12.99)](https://www.amazon.com/DIYMAG-Refrigerator-Magnets-100-piece/dp/B0753ZPBLQ/ref=sr_1_15?crid=1LP6OMWHOW7J0&dib=eyJ2IjoiMSJ9.WlU1gPXNyLeoE60GeE-rIFVgLx09JrIzCqVNNmZI45Se5J-RxH5oeplSl2VZjbZazxosP3Ww3WEyXQRheL1tMhdbiS9NHFA3k4PDUAtjCQ_pDsDKOdLYM4CulMzqCWwsFtrzBy6IabptRBPHUnjV77nJ0TB0FTenl1IaVMa2_x4l9SJvljne80_YfM-Is8V8TxyEISlLSXDLJCjZRkrJcUHff_Wv2qCz67dz7HNRva4.WYhowoa9txxhU4kfoz_R9glKt7drWcm2iIcKx4Yotcc&dib_tag=se&keywords=10mm%2Bdiameter%2Bmagnets%2Bneodymium&qid=1737917543&sprefix=10mm%2Bdiameter%2Bmagnets%2Bneodynium%2Caps%2C114&sr=8-15&th=1
) 

You can use different YubiKeys with this set up, but I prefer the C Bio series personally; it's more compatible with my other devices due to the USB-C port and I like only having to use a fingerprint to access my devices. You can also use magnets you have available already, as I did here.

# Case

![Image_1](https://github.com/user-attachments/assets/31b4529a-aee6-4a91-a84c-dbc4814b778e)


The 3D-printed case is shown in this section. I simply have it on the most accessible side of my desk (beneath the righthand side of it).

![Image_2](https://github.com/user-attachments/assets/dd2a7c67-5f6e-42c9-842a-82bc16e864a3)

## Specifications & Material(s)
Below you can find the printer and material used.

![image](https://github.com/user-attachments/assets/745c27a2-e1c1-4e25-8483-ed48dd09cdd9)

### 3D Printer
 Original Prusa Mini+
### Material(s)

* [INLAND Marble PLA Filament ($29.99)](https://www.amazon.com/Inland-1-75mm-Marble-Printer-Filament/dp/B08M4733VV/ref=sr_1_3?crid=RY0788Z9D3XL&dib=eyJ2IjoiMSJ9.GvDUjGeacdaThMoKB2T31ewH9i3JmlLfhoDydChHBm-pD7cXPBEVjrKUewiIA1ZLE0_09V1n0PRn75b7hFqiDw4M0-lnl6NiRKwU4Bay_UQglrp8aVfnSITNRxxnTlk00zi7jk9JMRR5mzHilVguVNlu22jSBhxaIA2Mgu28qpM98QySMqZ0onKGj8rI2Ae99hyhSl7nTwlWuBccngRzfk5tlxoLLDb3Ck8adz-NTaQ.5vcyT03Wl1FkUx1DENvwhSOMvdqbl_TQCjXICAq7kSI&dib_tag=se&keywords=pla+filament+inland+marble&qid=1735843633&sprefix=pla+filament+inland+marble%2Caps%2C87&sr=8-3) 

### Software
 PrusaSlicer

![Image_3](https://github.com/user-attachments/assets/f2f82253-fe65-4fad-910f-25885510eb41)


#### Settings
  Layer Height: .2mm \
  Infill: 30% \
  Supports: Everywhere \
  Estimated Printing Time: 1 hour and 55 minutes

# Setup for Linux

I am using ZorinOS as my primary OS at the moment across all my devices. Since it is a Debian-based distribution, this makes it easy to find guides for adding the second level of authentication. I used a guide available here: https://support.yubico.com/hc/en-us/articles/360016649099-Ubuntu-Linux-Login-Guide-U2F.

## Configuring Fingerprints (YubiKey C Bio - FIDO Edition)

This is specific to my key, but something similar will likely need to be done for other keys. I downloaded Yubico Authenticator through Flathub.

![Image_4](https://github.com/user-attachments/assets/643e5d76-d40a-495e-b914-94fd497402d6)

You can use this to setup your fingerprints. Plug in your key, you will then see information and a place to add your fingerprints; do so and here are the fingers I use:

![Image_5](https://github.com/user-attachments/assets/ba749d41-e8d5-4cd2-872b-adea1a6acdf6)


Once you have set up your fingerprints, you can move on to the next section.

## Configuring Key to Your Account

In terminal, follow these steps:

1. Run:
```bash
sudo apt-get install libpam-u2f
```
2. Insert your U2F Key (if you haven't already)
3. Run:
```bash
mkdir -p ~/.config/Yubico
```
3. Run:
```bash
pamu2fcfg > ~/.config/Yubico/u2f_keys
```
4. You will be prompted to touch your key if using the Bio series, which I am; do so when the key is flashing green.
5. To test if it works, open up a new terminal and run:
```bash
pamu2fcfg -n >> ~/.config/Yubico/u2f_keys
```
6. When prompted, you should see the flashing again and touch the key.

WARNING: If you lose the key, depending on how you modify the file to access the computer, you may no longer be able to access your computer.

### Adding as a Requirement for Sudo
If you would like to have the key be required to run sudo, please do the following:

1. Open up a new terminal and run:
```bash
sudo nano /etc/pam.d/sudo
```
2. Add the following line below the "@include common-auth" line.
```bash
auth       required   pam_u2f.so
```
![Image_6](https://github.com/user-attachments/assets/bbb21e06-d45b-428d-9f2f-cf3fa8c7c086)

3. When done, press Ctrl+X, then Y, then Enter.

### Adding as a Requirement for Logging In
This is probably what you came here for.

1. Open up a new terminal and run:
```bash
sudo nano /etc/pam.d/gdm-password
```
2. Add the following line below the "@include common-auth" line.
```bash
auth       required   pam_u2f.so
```
![Image_7](https://github.com/user-attachments/assets/588d736f-7472-4b7e-be56-709f95abad7f)

3. When done, press Ctrl+X, then Y, then Enter.

# Tips
If you wish to allow for the option of either password or password + key, change "required" to "optional" in step 2 of Adding as a Requirement for Logging In. Please note that it will only require password if no key is inserted, but will prompt for fingerprint if key is inserted. This isn't really practical though.

I used hot glue to attach the magnets, but gorilla glue works pretty well too. I made sure they attracted when put in with the case.

The fit for the USB C angled part is a bit tight, but tighter is better so it holds up to constant pushing. I also recommend maybe having a bit of filler on the other side, like some cardboard, wood, or PLA discards to prevent the USB-C facing forward from too much backward motion.

When taking out the YubiKey, I usualy hold the right side of the cover. I would hot glue the cover or made it tighter, but I would want to be able to easily disassemble if needed.
