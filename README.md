import qrcode as qr#pip install qrcode
from PIL import Image
#making variable img and insert link oy youtbe link in make fuction so it can make qr code 
img=qr.make("https://youtu.be/B_I-JMKzAHA?si=qv6VvUpIv0AvgEfg")
img.save("MrCodey.png")
qr=qr.QRCode(version=1,
             error_correction=qr.constants.ERROR_CORRECT_H,
             box_size=10,border=10)
qr.add_data("https://youtu.be/B_I-JMKzAHA?si=qv6VvUpIv0AvgEfg")
qr.make(fit=True)
img=qr.make_image(fill_color="black",back_color="white")
img.save("MrCodey.png")
