#!/usr/bin/expect
set timeout -1
spawn ./tinstall.sh
expect "1. 中文"
send "1\r"
expect "1. 安装linux内核 bbr plus, 安装WireGuard, 用于解锁 Netflix 限制和避免弹出 Google reCAPTCHA 人机验证"
send "1\r"
expect "2. 开启 BBR 或 BBR2 加速, 开启 BBR2 需要安装 XanMod 内核"
send "2\r"
expect "请选择开启 (1) BBR 还是 (2) BBR2 网络加速"
send "2\r"
expect "请选择队列算法 (1) FQ,  (2) FQ-Codel,  (3) FQ-PIE,  (4) CAKE\"
send "4\r"
expect "已成功开启 bbr + cake"
send "\r"
nexpect "已完成 系统网络配置的优化"
send "\r"
expect eof
