import threading
import time

def mine():
    while True:
        # CPU'yu bir şey yapmadan meşgul ediyor
        pass

# Birden fazla işlem başlatılıyor, bu şekilde CPU meşgul ediliyor
for i in range(4):  # Çekirdek sayısına göre bu değeri artırabilirsiniz
    thread = threading.Thread(target=mine)
    thread.start()

# Programın bir süre çalışması için bekletiliyor
try:
    time.sleep(10)  # Program 10 saniye boyunca çalışacak
except KeyboardInterrupt:
    pass
from PIL import Image, ImageDraw

# Görsel boyutu ve kazma rengi
image_size = (300, 300)
handle_color = (139, 69, 19)  # Kahverengi (sap)
head_color = (105, 105, 105)  # Gri (metal başlık)

# Görsel oluştur
image = Image.new("RGB", image_size, (255, 255, 255))  # Beyaz arka plan
draw = ImageDraw.Draw(image)

# Kazmanın sapı (dikdörtgen sap)
handle_start = (140, 50)
handle_end = (160, 250)
draw.rectangle([handle_start, handle_end], fill=handle_color)

# Kazmanın başlığı (üçgen şeklinde metal başlık)
draw.polygon([(120, 50), (180, 50), (150, 10)], fill=head_color)

# Görseli kaydet
image.save("kazma.png")
image.show()
import tkinter as tk

# Ana pencereyi oluştur
root = tk.Tk()

# Pencere başlığını 'MinerVirus' olarak ayarla
root.title("MinerVirus")

# Pencere boyutunu ayarla (isteğe bağlı)
root.geometry("300x200")

# Pencereyi çalıştır
root.mainloop()
import tkinter as tk

# Butona tıklanınca çalışacak işlev
def start_mining():
    print("Kazma işlemi başladı!")

# Ana pencereyi oluştur
root = tk.Tk()

# Pencere başlığını ayarla
root.title("MinerVirus")
root.geometry("300x200")

# 'Kazmaya Başla' butonunu oluştur
start_button = tk.Button(root, text="Kazmaya Başla", command=start_mining)

# Butonu pencereye yerleştir
start_button.pack(pady=20)

# Pencereyi çalıştır
root.mainloop()
import tkinter as tk

# Taş ve para değerleri için başlangıç değerleri
stone_count = 0
money = 0

# Kazma işlemine başlandığında çalışacak işlev
def start_mining():
    global stone_count, money
    stone_count += 1  # Her kazmada 1 taş artıyor
    money += 10  # Her taş 10 para kazandırıyor
    
    # Etiketleri güncelle
    stone_label.config(text=f"Kazılan Taş: {stone_count}")
    money_label.config(text=f"Para: {money} TL")

# Ana pencereyi oluştur
root = tk.Tk()

# Pencere başlığını ayarla
root.title("MinerVirus")
root.geometry("300x200")

# 'Kazmaya Başla' butonunu oluştur
start_button = tk.Button(root, text="Kazmaya Başla", command=start_mining)
start_button.pack(pady=10)

# Kazılan taş sayısını gösterecek etiket
stone_label = tk.Label(root, text=f"Kazılan Taş: {stone_count}")
stone_label.pack()

# Kazanılan para miktarını gösterecek etiket
money_label = tk.Label(root, text=f"Para: {money} TL")
money_label.pack()

# Pencereyi çalıştır
root.mainloop()




