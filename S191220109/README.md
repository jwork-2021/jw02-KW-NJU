# W02-S191220109

## 任务一
1.
example类图（建模）如下：
![](http://www.plantuml.com/plantuml/png/RP7BJiGm34Nt_eei0Mdc4z0mczcmG3pO81PkQqf5caHv28R7lnF5SGZITDFhs_Z4ljs5Y3wcLGCi9f9_mP7KzM9mqFG5AZ-1ueqDIroiEJilpdpAUKITA9S_FUZE-YoPeorEzNZ8TiVIQBYHJ5hLmIO_SKi6AT_KtDHGbCoWN1KWn8BO7s_HlDLh_9yCx-YabQyTDORGS7nrZK1fVaiIrUxxiaMAcmJnzDnc2ZoKIzt2LKLxvJqUUzQ1w5FoOgtYAx4g9WTQ0goEGE_bdAn9aG_NEYz23wuM3dqWphtKz45ZYl_MsgSXByg8zZVoOiXpHB-OMRcCW9OgjvVmrNRxVIaX0lGm_iGQeAItsLoqx01sPAQqwby0)

example执行时序图（建模）如下：
![](http://www.plantuml.com/plantuml/png/ZPBBgjD07CRtynI1hdq15t8u6xVkN8Z8d3gqmMbI9WbILn5CBzfBxIMnK2dLLaLH2XKliS5taSoOleNJP2AJa8PJkWYJt_V_Vz-NkJ1CI4ohWG6icZfHabzaFwMRh_m16aeDeISeVb6vnB3wICcIBpz5pzzHvnazh9H4K8KONa6Z_k2Aw2VL7OiqCL80qapLR2MouwjLU1Z4E5Orf5JkrbKJPH0sd72ABZx4bA4J4v4p7FL7pFt9rbtXe8cXLeXE1s6mPDwM_lO4YlLQ4HbzsT5WdYv_J5HfEOWTtxXNkKqGqkxVIXBSL6ZNuuO1oEJds2Msa4GvsvWIjKfZn0b7EZvT-W28p1AId70aUkj4GV37dl4_RK_OVYrgsCzpkXQNnNsS3Bwcxr_GlYjN9ZaHJgKjm-zqvFx_47bK2dMm-UHaR16brywjBt2RwI-DUdB0-rtxN5dQZ31njeI_inNhZiiR4Ap8NyxcxR9-JnOSxN7uusFeRzZWJJP3SKlYviat5G1n_wIuueIlwqrv-SpjXB--vS1MEbFakFPCkcid56ql-7KLmqiLplxeVKx12wGzj1hu7m00)

2.
好处：
(1)逻辑清晰，对象关系明确，每个对象在使用其它类时，都先将其它类对象装载到本类当中，明晰了对象概念，明确了对象间关系；
(2)代码易于扩充，接口的使用便于扩充更多同类功能，只需对原有代码进行少许修改即可实现（以添加多种排序算法为例）；
(3)代码码复用性好，基于类实现的面向对象将每个对象及功能函数进行封装，在需要添加已有类的对象时，无需大量修改代码即可直接使用；
(4)用类来定义对象，能够更好地模拟实际场景，使得事件发生过程更清晰，每个对象的独立行为与交互行为更为明确。

可改进之处：
(1)发现bug：example代码在应对初始即为有序序列时，会出现读取空字符串报错；
(2)跨类装载等操作过多，致使类间关系更加复杂，代码易读性降低；
(3)代码扩充不够灵活，已经定义的接口会限制了继承类中重载函数的参数个数，致使无法根据继承类的特性定义更符合使用习惯的函数，甚至可能导致部分功能无法实现（以本例中无法使用需要函数参数的递归类排序为例）;
(4)移植性较差，生成的txt文件需要特定的插件对其进行读取并展示为可视化界面，导致程序的可移植性与独立性降低。

## 任务二
S191220109.task2类图（建模）如下：
![](http://www.plantuml.com/plantuml/png/dL9BJWCn3Dtx55a2Kdi4L5Y312gmGImyKpED9fD4-GXGuUu4vwECn0QwQ9u_VlQpP-S3kX0N1I1r8FUA8uaRgN5GT0AHVfx2dV4oIAFFpjap_UPvGXKfcLyzqTwu13EFCdWewJwvEow5EXUE2hqNjqRxLfMuX6jeQcXeICV5ePxPhcC9Mm2m-oTUMx-XhLbzq-hBNSi8Oialr4MKnVI5oKNYjEh-_DBwUmxmdusTveA2kN8EFtg-lSQvR9wX24TYmAwyKE7vWShsK5AgHWevhzWgZVXeYs7HUSehPvlUQOnX9Uaw3abafcXNIA8mZn2Sr9EmYGBQIllo-oZ7-U_LHVwHbFf7wtgnxVRpidw_04r92sKCq0sv3dG3h0DywCtcefqPO4Vw41Vr3G00)

可视化结果展示链接:
(1)冒泡排序
[![asciicast](https://asciinema.org/a/438475.svg)](https://asciinema.org/a/438475)
(2)希尔排序
[![asciicast](https://asciinema.org/a/438471.svg)](https://asciinema.org/a/438471)
(3)快速排序
[![asciicast](https://asciinema.org/a/438339.svg)](https://asciinema.org/a/438339)

## 任务三
代码主要改动：添加Line的继承类Matrix类，重载toString函数，实现换行输出。
S191220109.task3类图（建模）如下：
![](http://www.plantuml.com/plantuml/png/dLBBJWCn3BpxAt84fFOJKE4C4gZ01N5mjwPTDPj4UOYYmh_ZnacKbRX03ztnn1vxdAn2H1_Jf0564yc_uq3gRZIuqNG2nRz0yS66COxMN5ncPlSRyu8w4OVVlT3QUeQYeorkItfWkjFIQAHmq1Y2khScj2hMKhwXNKERXaoQF9f3ZkjOoXK0cJwVrzOVw6fMtxHoqhMCe2RvGbr4MKnVo1Ifqwpxwrlh7_91_dEfyrnGj3VUu-VCFKO_7ckqDdYGUn2eufuo42glLuNyWQhzL59yjKnH4akiUU9dLmA7Ff3SG8xfI4EACuUtQSEUHQ9T2dj4cO77DJlbM0BQXllonpGEXxzN5_zxqleVhUi5BfTVr_Kv0yXkrM8X93FDMqiM3D2DFJ_eHfeVd1LP-wgz0u0LcMsQz0y0)

可视化结果展示链接:
(1)冒泡排序
[![asciicast](https://asciinema.org/a/438484.svg)](https://asciinema.org/a/438484)
(2)希尔排序
[![asciicast](https://asciinema.org/a/438482.svg)](https://asciinema.org/a/438482)
(3)快速排序
[![asciicast](https://asciinema.org/a/438479.svg)](https://asciinema.org/a/438479)
