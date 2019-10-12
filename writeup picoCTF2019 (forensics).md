# Write up picoCTF 2019 (forensics)

## Challenge 1: Glory of the Garden

Link chall: [Challenge1](https://2019shell1.picoctf.com/static/38b5c0bde1a6a92d282b128c71799722/garden.jpg)

Vừa nhìn vào hint: "What is a hex editor" lập tức chúng ta sẽ nghĩ đến tool HxD để check xem các mã hex bên trong file đề bài cho có gì không :v

![](https://scontent.fsgn4-1.fna.fbcdn.net/v/t1.15752-9/72565814_2477879202534534_3521698222932230144_n.png?_nc_cat=107&_nc_oc=AQnpXuX_tErxiAI6VOtFs0YvBJxvIgZ3j64b3RP6YEkwkMOlIzkwUSRQcI2wm6PUiBjzxtq5A8o1kweUmbFGFFPD&_nc_ht=scontent.fsgn4-1.fna&oh=aeacfb0dd51535846e3cfd6026a17c1e&oe=5E280F52)

Thì thấy header không có gì thay đổi cả, thử ctrl +F search thử picoCTF xem 

WELL!!!

![](https://scontent.fsgn4-1.fna.fbcdn.net/v/t1.15752-9/72567296_705864756600715_2546869126391922688_n.png?_nc_cat=103&_nc_oc=AQkoaWxVkkaAklZlNy4fOJhdnnmMnuWVimMHj3GiMFv2gicYW0sR5PwQkm89uVAzCHfyf7LOa8PD70zTpUm4vA8I&_nc_ht=scontent.fsgn4-1.fna&oh=f1f96267ced8a95178e176cf45eb0972&oe=5E2C52FE)

Flag: picoCTF{more_than_m33ts_the_3y36BCA684D}

## Challenge 2: Unzip

Link chall: [Challenge2](https://2019shell1.picoctf.com/static/37762a7e5774d7d6c1bc79e8e1758ef9/flag.zip)

Thấy tên đề là đủ hiểu là extract file zip rồi :v

1.Nhấp chuột phải vào file chọn extract here 

2.vào cmd > unzip file.zip

Flag: picoCTF{unz1pp1ng_1s_3a5y}

## Challenge 3: Meta data

Link chall: [Challenge3](https://2019shell1.picoctf.com/static/ddffae2f670f7c822c4f878e932bf6c5/pico_img.png)

Chall này muốn chúng ta biết cách đọc dữ liệu trong file

![](https://scontent.fsgn4-1.fna.fbcdn.net/v/t1.15752-9/72085277_525720308205099_4177857054100160512_n.png?_nc_cat=102&_nc_oc=AQkWpTGMILp6rrAhyxrE5yyoDRvm07dVVTLqLZen1FUI_SpG4OTC4eWqdhQGoAiYVOKsUsIqGr4WGTXos4pDo3i2&_nc_ht=scontent.fsgn4-1.fna&oh=847d4dc24dd8d7e74906fbab13f56699&oe=5E1FCE7A)

![](https://scontent.fsgn4-1.fna.fbcdn.net/v/t1.15752-9/71876060_661797504329864_7518111561819357184_n.png?_nc_cat=100&_nc_oc=AQkL2PVx39CSW0L6Cn6VjV4c26arCJSPIoxh6EKHFmbseSLPkAiujdT61NTCsI-_I7-FaBTtomjvvZhbDAPxDlKN&_nc_ht=scontent.fsgn4-1.fna&oh=6d292c02ba297084e87e38276b5fdc56&oe=5E371B0C)

Flag:picoCTF{s0_m3ta_dc38ce45}

## Challenge 4: What Lies Within
Link chall:[Challenge4](https://2019shell1.picoctf.com/static/aec3861fc4d5bce4d39dc0db196426de/buildings.png)

Sử dụng stegonoraphy online để hide message trong image

![](https://scontent.fsgn4-1.fna.fbcdn.net/v/t1.15752-9/72749406_2495597143860439_7067909228677038080_n.png?_nc_cat=103&_nc_oc=AQl3SmsxVlIR6ssqd4BDTIQ70vkairHBfecT9iCka620NRvB3qrzCpf0UItRGvFnsMtqVzfR6bS72OV0FbcRo58U&_nc_ht=scontent.fsgn4-1.fna&oh=31f55c13c283cf1efa6f43559cbf842e&oe=5E35F0A5)

Flag: picoCTF{h1d1ng_1n_th3_b1t5}

## Challenge 5: extensions

Link chall: [Challenge5](https://2019shell1.picoctf.com/static/45886ed4b6d5d1dc74c4944fcf4b4041/flag.txt)

Extensions hiểu đơn giản là phần mở rộng của file, dựa vào hint thì chắc chắn chúng ta có thể suy luận rằng phần mở rộng của file đã bị thay đổi. Vậy nên chúng ta hãy sử dụng câu lệnh file để kiểm tra xem nó thuộc loại file nào

![](https://scontent.fsgn4-1.fna.fbcdn.net/v/t1.15752-9/72262138_1394861680670390_2422408430217068544_n.png?_nc_cat=108&_nc_oc=AQlUGMnSMH3dYqG2rhzGmNV7I_ii7wr5TcmqMxhc_LZ7LopT3W8jlo18Ifr-emCZXe7o7_Jjon8X94QGi7kgshUk&_nc_ht=scontent.fsgn4-1.fna&oh=cafa2657c588ced62bbc9031667e45d5&oe=5E2D73E8)

Vậy đây là file png, chúng ta chỉ cần đổi sang flag.png là sẽ thấy flag

Flag: picoCTF{now_you_know_about_extensions}

## Challenge 6: shark on wire 1

Link chall: [Challenge6](https://2019shell1.picoctf.com/static/ae9ca8cff43ed638ed5d137f9ece7455/capture.pcap)

Cứ thấy file pcap thì chắc chắn chúng ta nghĩ đến ngay wireshark, một công cụ khá mạnh để phân tích các giao thức trao thức trao đổi mạng

Khi vào thấy hint thì thấy gợi ý về stream và đề bài này muốn nhắc đến UDP stream =>follow>UDP stream

![](https://scontent.fsgn4-1.fna.fbcdn.net/v/t1.15752-9/72212383_525731144909366_7940624721840701440_n.png?_nc_cat=100&_nc_oc=AQm9JfWTMSaiBydl99WkSBcsV8ryzs8_EBdLWzo1tYmV4pKhfNY7e32jZ4wAf3ELgvIeSh3Z8M9Gfx2ihBCuTDTS&_nc_ht=scontent.fsgn4-1.fna&oh=d432b0bbc487b18f3026c3671670fcf4&oe=5E18C568)

Flag: picoCTF{StaT31355_636f6e6e}

## Challenge 7: like 1000

Link chall: [Challenge7](https://2019shell1.picoctf.com/static/8694f84879d3b7c0dcf775930f4665fc/1000.tar)

Đề bài cho là 1 file tar, nhiệm vụ của mình chỉ extract hết 1000 file tar đó là có được flag vậy nên mình sử dụng python để auto extract

```
import tarfile
i=999
while i>0:
 	tf=tarfile.open(str(i)+".tar")
 	tf.extractall()
 	print("File"+str(i)+".tar is decompressed")
 	i=i-1
```
Flag: picoCTF{l0t5_0f_TAR5}

## Challenge 8: shark on wire 2

Link chall: [Challeng8](https://2019shell1.picoctf.com/static/dcd259894e0efe9d6e91da2af47e6369/capture.pcap)

Đây là dạng file pcap giống challenge1 nhưng khi mình vào UDP stream thì không thấy flag như challenge1 nữa nhưng có 1 điều khá đặc biệt ngay địa chỉ 10.0.0.66

![](https://scontent.fsgn4-1.fna.fbcdn.net/v/t1.15752-9/72635268_2068303333269334_6399118860036866048_n.png?_nc_cat=100&_nc_oc=AQkS-znXkhahuiebFrU2y3gob_jxoArpgQreW24rC8noJz0IH-hhyMPMZGFtbMzSWe8AqAhgYH7FBvrPpXUICz07&_nc_ht=scontent.fsgn4-1.fna&oh=ed0f32430010cf1a55e6efcfb961b045&oe=5E3A7EBA)

Khi bạn thử tăng stream lên thì thấy các dòng chữ a theo có length khác nhau và có vẻ như theo 1 trình tự nào đó

Khi mình sort theo thứ tự

![](https://scontent.fsgn4-1.fna.fbcdn.net/v/t1.15752-9/72373133_485494898974930_3281818325151121408_n.png?_nc_cat=111&_nc_oc=AQlmKdEM0WzZoNbP2esZAIQk3aYJYWo710wG91A-slsEWxP6uJmpMQJL1kt9SI5FUirzV_NVF90JSehn29hPufgi&_nc_ht=scontent.fsgn4-1.fna&oh=bcf0da912881e0c3a3d0caca5be06a5c&oe=5E1829DA)

Hãy để ý đến **length** các bạn sẽ thấy đều bắt đầu bằng số 5 và đằng sau số 5 ấy có vẻ như là asii. Vậy nên mình thử decode xem

![](https://scontent.fsgn4-1.fna.fbcdn.net/v/t1.15752-9/71727811_2288580368100229_5100672791015849984_n.png?_nc_cat=103&_nc_oc=AQmzr1s_ZiaUr2IJLhcmmyvfNFqYHuxsMkZQ-IHQdGyHEaO0E4I70qHEPNP7EZKW94BuIw1J32muuVGhsPsHxbv6&_nc_ht=scontent.fsgn4-1.fna&oh=4f3c145e7b18a6d5bb1d001dfbe29e71&oe=5E318417)

Flag: picoCTF{p1LLf3r3d_data_v1a_st3g0}


