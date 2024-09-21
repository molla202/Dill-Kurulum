![image](https://github.com/user-attachments/assets/384e0b28-bc2c-474d-ac29-eb361ca5b30a)

 * [Topluluk kanalımız](https://t.me/corenodechat)<br>
 * [Topluluk Twitter](https://twitter.com/corenodeHQ)<br>


| Network Name  | Dill Testnet Alps  |
| ------------- | ------------------ |
| Rpc URL       | https://rpc-alps.dill.xyz/ |
| Chain ID      | 102125             |
| Currency Symbol | DILL             |
| Explorer URL  | https://alps.dill.xyz/ |

# Hardware Requirements

| Node Type     | CPU    | Memory | Disk  | Bandwidth | OS Type |
| ------------- | ------ | ------ | ----- | --------- | ------- |
| Light Validator | 2 Cores | 2GB  | 20GB  | 8Mb/s     | Ubuntu LTS 20.04+ / MacOS |
| Full Validator  | 4 Cores | 8GB  | 256GB | 64Mb/s    | Ubuntu LTS 20.04+ / MacOS |


### Kurulum script

Not: dill takımı zaten hazırını ayarlamış yapacağınız şey tek kodu girip yönergeleri takip etmek.

```bash
curl -sO https://raw.githubusercontent.com/DillLabs/launch-dill-node/main/dill.sh && chmod +x dill.sh && ./dill.sh
```

### Validator Keys oluşturma

- Daha sonra, doğrulayıcı anahtarlarınızı oluşturmanız istenecektir. Yeni bir anımsatıcı oluşturabilir veya mevcut olanı kullanabilirsiniz.
- yeni key oluşturuyoruz.
- 3600 ligt 36000 ise validator node hangisi iseniz seçin.
- Para çekme adresiniz olarak bir Eth1 adresi belirliyorsunuz. Lütfen bu adresin kontrolünün sizde olduğundan emin olun

```bash
                       _______       __     __     __
                      |       \     (__)   |  |   |  |
                      |   ___  \     __    |  |   |  |
                      |  |   |  |   |  |   |  |   |  |
                      |  |   |  |   |  |   |  |   |  |
                      |  |   |  |   |  |   |  |   |  |
                      |  |___|  |   |  |   |  |   |  |
                      |        /    |  |   |  |   |  |
                      |_______/     |__|   |__|   |__|

Creating your keys.
Creating your keystores:	  [####################################]  1/1
Verifying your keystores:	  [####################################]  1/1
Verifying your deposits:	  [####################################]  1/1

Success!
Your keys can be found at: <YOUR_FOLDER_PATH>/dill/validator_keys
```

- Dosya yolunda key dosyamız oluştu.
- yönergeleri takip edip kurulumu bitirin.

- https://staking.dill.xyz/ adresine gidelim
- deposit işlemlerini buradan yapabiliyoruz.
- seçilmediğimden kuramadım farzı misal anlatıyorum. eksikler yanlışlar illaki olabilir.
- https://alps.dill.xyz/validators burdan valiyi kontrol edebilirsiniz.

### yararlı komutlar

```bash
./health_check.sh -v
```

- Doğrulayıcıların ortak anahtarını görüntüleyin
```bash
./show_pubkey.sh
```

- durdur dill node
```bash
./stop_dill_node.sh
```

- başlat dill node
```bash
./start_dill_node.sh
```

- yapmamalıyız sanırım :D
```bash
./exit_validator.sh
```

