# Tutorial nuyul bnb-miner.live

- buka browser chrome
- buka bnb-miner.live dan login address bnb mu suu
- masuk ke inspect elemen. 
- pilih tab console
- copy code dibawah ini


``
let formData = new FormData;
formData.append('action', 'claim');
for(let i = 0; i < 1000; i++){
        console.log("gass");
        fetch('https://bnb-miner.live/ajax.php', {
        method: 'POST',
        body: formData
        })
        .then((response) => response.json())
        .then((result) => {
            console.log(result);
        })
        .catch((error) => {
            console.error('Error:', error);
        });
}

``
