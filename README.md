function func(s, a, b) {

  if (!s) return -1;

  const aIndex = s.lastIndexOf(a);
  
  const bIndex = s.lastIndexOf(b);

  if (aIndex == bIndex) return -1;

  const maxIndex = Math.max(aIndex, bIndex);

  if (maxIndex == s.length) {
  
    return Math.min(aIndex, bIndex);
    
  }

  return maxIndex;
  
}
