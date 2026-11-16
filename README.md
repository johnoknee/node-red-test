let data = msg.payload;
let temp = data.temp;

let status = "safe";
let fanon = false;

if (temp > 9) {
    status = "fire";
    fanon = true;
}

let msg1 = {
    payload: temp
};

let msg2 = {
    payload: status
};

return [msg1, msg2];
