const PushBullet = require('pushbullet');
const pusher = new PushBullet('YOUR-API-KEY');

// Retrieve a list of pushable devices
pusher.devices((error, response) => {
    // Handle the response (JSON)
});

// Push a note to a specified device
pusher.note('device_iden', 'New Note', 'Note body text', (error, response) => {
    // Handle the response (JSON)
});
