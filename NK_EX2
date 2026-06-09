function findMaxBlockSum(str) {
    const blocks = str.split('0').filter(block => block.length > 0);
    if (blocks.length === 0) {
        return "Нет блоков, разделенных нулями";
    }
    let maxSum = -1;
    let maxBlock = "";
    
    for (const block of blocks) {

        let sum = 0;
        for (const digit of block) {
            sum += parseInt(digit, 10);
        }
        
        if (sum > maxSum) {
            maxSum = sum;
            maxBlock = block;
        }
    }
    return `${maxBlock}, ${maxSum}`;
}
const example = "012340123017210112432";
console.log(findMaxBlockSum(example));
