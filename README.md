function chunkArrayInGroups(arr, size) {
  let temp = [];
  while(arr.length > 0) {
    temp.push(arr.slice(0, size));
    arr= arr.slice(size);
  }
  return temp;
}

chunkArrayInGroups(["a", "b", "c", "d"], 2);
