import { useState } from "react";

function App() {
  const [amount, setAmount] = useState("");
  const [paid, setPaid] = useState(false);

  function payment() {
    if (amount > 0) {
      setPaid(true);
    } else {
      alert("Enter amount");
    }
  }

  return (
    <div style={styles.container}>
      <h1>Payment System</h1>

      <input
        type="number"
        placeholder="Enter Amount"
        value={amount}
        onChange={(e) => setAmount(e.target.value)}
        style={styles.input}
      />

      <select style={styles.input}>
        <option>UPI</option>
        <option>Credit Card</option>
        <option>Debit Card</option>
        <option>Cash</option>
      </select>

      <button onClick={payment} style={styles.button}>
        Pay Now
      </button>

      {paid && (
        <h3 style={{ color: "green" }}>
          Payment of ₹{amount} Successful!
        </h3>
      )}
    </div>
  );
}

const styles = {
  container: {
    width: "350px",
    margin: "100px auto",
    padding: "30px",
    textAlign: "center",
    fontFamily: "Arial",
    boxShadow: "0 0 10px #aaa",
    borderRadius: "10px"
  },

  input: {
    width: "90%",
    padding: "12px",
    margin: "10px",
    fontSize: "16px"
  },

  button: {
    padding: "12px 30px",
    background: "blue",
    color: "white",
    border: "none",
    borderRadius: "5px",
    cursor: "pointer"
  }
};

export default App;
