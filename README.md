# application
let a1 = [['a',1],['b',1],['c',1],['a',2],['b',2],['c',2],['a',3],['b',3],['c',3]]
console.log([...new Set(a1.map(i=>i[0]))].map(j=>[j,...[...new Set(a1.map(k=>k[0]===j?k[1]:''))].filter(s=>s)]))
