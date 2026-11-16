let data = msg.payload;
let temp = data.temp;

let status = "";
let fanon = false;

if (temp > 9 ){
    status ="fire";
    fanon = true;
}
let msg1 = {
    payload: temp,
    status: status,
};


return msg1
