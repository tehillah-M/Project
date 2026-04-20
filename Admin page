import { useState } from "react";
import axios from "axios";

function Admin() {
  const [sport, setSport] = useState("");
  const [time, setTime] = useState("");

  const addSlot = async () => {
    await axios.post("http://localhost:5000/api/slots", {
      sport,
      time
    });
    alert("Slot Added");
  };

  return (
    <div>
      <h2>Admin Dashboard</h2>
      <input placeholder="Sport" onChange={e => setSport(e.target.value)} />
      <input placeholder="Time" onChange={e => setTime(e.target.value)} />
      <button onClick={addSlot}>Add Slot</button>
    </div>
  );
}

export default Admin;
