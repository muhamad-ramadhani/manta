
<p style="font-size:14px" align="right">
<a href="https://t.me/PemulungAirdropID" target="_blank">Join our telegram <img src="https://user-images.githubusercontent.com/72949170/194228482-0f875615-e155-4b12-8716-8111addd6cba.jpg" width="30"/></a>
</p>

<p align="center">
  <img width="60%" height="auto" src="https://user-images.githubusercontent.com/72949170/204498552-f289ce7c-2b59-4ff6-9442-99c4770af2eb.png">
</p>

# MANTA TRUSTED SETUP

## 1. Install 

```
source ~/.profile
```
```
curl --proto '=https' --tlsv1.2 -sSf https://raw.githubusercontent.com/Manta-Network/manta-rs/main/tools/install.sh | sh
```
```
manta-trusted-setup register
```

![image](https://user-images.githubusercontent.com/72949170/204499260-1e97c2d4-6d5c-4db5-8128-c734734777f9.png)

**SIMPAN INFORMASI WALLET KALIAN**

## 2. Isi Form
- Buka link form yang tadi nongol saat instal
- Isi detail kalian + alesan ikutan
- Submit address calamari kalian

> Cara dapet address
> Pergi ke https://polkadot.js.org/apps/#/settings/metadata
> Ganti chainnya yang di menu drop-down sebelah kiri, cari Calamari chain terus switch
> Ke menu setting terus update metadata
> Balik ke wallet polkadot, klik yang titik 3 terus ganti chain ke Calamari Parachain
> Done, depannya 'dm'

## 3. Run Contributor
Setelah isi form dan wallet kalian berhasil terdaftar lanjut step berikut

```
sudo apt update
```
```
sudo apt install pkg-config build-essential libssl-dev curl jq
```

Install Rust
```
curl https://sh.rustup.rs/ -sSf | sh -s -- -y
```
## 4. Setting Path
```
source $HOME/.cargo/env
```
## 5. Install Manta-RS
```
git clone https://github.com/Manta-Network/manta-rs.git
```

## 6. Installation
```
screen -S manta
```
```
cd manta-rs
```
```
cargo run --release --all-features --bin groth16_phase2_client contribute
```

![image](https://user-images.githubusercontent.com/72949170/204500861-5c729858-e331-4a6b-b18f-e91c6686cdee.png)

Masukan Pharse pas saat registrasi

## DONE, UNTUK UPDATE SELANJUTNYA KALIAN BISA PANTAU <a href="https://t.me/PemulungAirdropID" target="_blank">CHANNEL KITA </a>

## Perintah berguna (bukan bagian dari tutorial)

Enter Screen
```
screen -Rd manta
```

Hapus Directory
```
rm -rf manta-rs
```
