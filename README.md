# REACT-NATIVE

### console.log() 

RUN IN TERMINAL

```
$. react-native log-android
```

### handleChange and handleSubmit

```
const [enteredGoal, setEnteredGoal] = useState('');

  const handleChange = inputText => {
    setEnteredGoal(inputText);
  };

  const handleSubmit = () => {
    console.log(enteredGoal);
  };

  return (
    <View style={styles.screen}>
      <View style={styles.header}>
        <TextInput
          placeholder="Add Goals"
          style={styles.input}
          onChangeText={handleChange}
          value={enteredGoal}
        />
        <Button title="ADD" onPress={handleSubmit} />
      </View>
    </View>
  );
};
```
