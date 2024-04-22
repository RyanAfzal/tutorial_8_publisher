# Tutorial 8

### Refleksi
1. Jumlah data yang dikirimkan oleh publisher ke message broker dalam satu kali run adalah lima pesan karena ada 5 pemanggilan publish_event yang di mana setiap publish_event mengirimkan sebuah UserCreatedEventMessage ke message brocker.
2. Arti amqp://guest:guest@localhost:5672 yang juga digunakan oleh subscriber artinya subscriber dan publisher terhubung ke server AMQP yang sama dengan kredensial yang sama (nama pengguna: "guest", sandi: "guest"), dan server berjalan pada localhost dengan port 5672.

<img width="949" alt="RabbitMQ" src="https://github.com/RyanAfzal/tutorial_8_publisher/assets/137851158/d4aae02f-b2ff-439d-9a30-37c749bc848b">


ss terminal publisher
<img width="801" alt="ss terminal publisher" src="https://github.com/RyanAfzal/tutorial_8_publisher/assets/137851158/d4df8a75-a591-4b1d-9513-6c2fb522a694">

ss terminal subscriber ketika telah berhasil menerima 5 event message broker dari publisher
<img width="738" alt="ss terminal subscriber" src="https://github.com/RyanAfzal/tutorial_8_publisher/assets/137851158/cf10611a-5865-41d8-b171-3fac8f6b5ab3">

Screenshot RabbitMQ saat terdapat spikes yang menandakan telah dijalankannya publisher dengan cargo run berkali-kali (message rates)
<img width="941" alt="ss chart adpro" src="https://github.com/RyanAfzal/tutorial_8_publisher/assets/137851158/797b5931-e4b1-42d0-be45-8f9262367354">
