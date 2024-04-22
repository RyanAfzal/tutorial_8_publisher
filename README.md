# Tutorial 8

### Refleksi
1. Jumlah data yang dikirimkan oleh publisher ke message broker dalam satu kali run adalah lima pesan karena ada 5 pemanggilan publish_event yang di mana setiap publish_event mengirimkan sebuah UserCreatedEventMessage ke message brocker.
2. Arti amqp://guest:guest@localhost:5672 yang juga digunakan oleh subscriber artinya subscriber dan publisher terhubung ke server AMQP yang sama dengan kredensial yang sama (nama pengguna: "guest", sandi: "guest"), dan server berjalan pada localhost dengan port 5672.

https://github.com/RyanAfzal/tutorial_8_publisher/issues/1#issue-2255748390