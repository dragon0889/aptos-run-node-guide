Cài đặt theo thao khảo tù guru.com.
Thời gian cài đặt tầm 10 phút.

Bước 1: cài đặt screen và chạy lệnh
>screen -S aptos

Bước 2: chạy scrip dưới đây

>wget -q -O aptos.sh https://api.nodes.guru/aptos.sh && chmod +x aptos.sh && sudo /bin/bash aptos.sh

Sử dụng bot telegram để tracking tại đây [telegram bot.](https://t.me/NodesGuru_bot)

Kiểm tra log
>journalctl -u aptosd -f

Khởi động lại node:
>systemctl restart aptosd

Hiển thị khóa cá nhân:
>cat ~/.aptos/key/private-key.txt

Hiển thị peer-id và public key:
>cat ~/.aptos/config/peer-info.yaml

Cập nhập node:
>wget -q -O aptos_update.sh https://api.nodes.guru/aptos_update.sh && chmod +x aptos_update.sh && sudo /bin/bash aptos_update.sh

Xóa node:

>systemctl stop aptosd
>systemctl disable aptosd
>rm -rf ~/aptos*
>rm -rf ~/.aptos
>rm -rf /opt/aptos/

Kiểm tra trạng thái node bằng cách nhập IP tại đây:

https://node.aptos.zvalid.com/

https://www.nodex.run/aptos_test/

https://status.devnet.aptos.dev/ 
