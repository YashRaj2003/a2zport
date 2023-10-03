function findlongestword(sentence) {
    const words = sentence.replace(/[^a-zA-\s]/g, '').split(/\s+/);

    let longestword = '';
    let wordwithvowels = '';

    for (const word of words) {
        const vowels = word.match(/[aeiouAEIOU]/g);
        const vowelCount = vowels ? vowels.length : 0;
        if (word.length > longestword.length) {
            longestword = word;
            wordwithvowels = word;
        }
        else if (word.length === longestword.length && vowelCount > wordwithvowels.match(/[aeiouAEIOU]/g).length) {
            wordwithvowels = word;
        }
    }
    return wordwithvowels;
}

// const sentence = "Smart people learn from everything and everyone, average people from their experience, stupid people already, have all the answers";
const sentence = "Sigleword";
console.log(findlongestword(sentence))
