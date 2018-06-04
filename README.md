# DictionaryFairy
Dictionary Tools and Shortcuts

### Class
```Python
class dictionaryFairy(object):
```

### Generate Dictionary With Zip
```Python3
    #Create Dictionary with a Zip and Loop approach
    def createDictLoop(self, keys, values):
        zipper = zip(keys, values)
        outDict = {}
        for k, v in zipper:
            outDict[k] = v
        return outDict
```

### Generate Dictionary with Comprehension
```Python3

    #Create a Dictionary with a Dictionary Comprehension approach
    def createDictComprehension(self, keys, values):
        zipper = zip(keys, values)
        outDict = {k:v for (k, v) in zipper}
        return outDict
```

### Generate Dictionary with a Dict(Zip())
```Python3
    #Create a Dictionary directly with a dict(zip()) approach
    def createDictDirect(self, keys, values):
        outDict = dict(zip(keys, values))
        return outDict
```

### Comparing Dictionaries
```Python3
    #Compare Dictionary sizes, return the larger 
    def compareDicts(self, dict1, dict2):
        d1 = len(dict1)
        d2 = len(dict2)
        
        # Check if both dictionaries are empty
        if not d1 and not d2:
            print("No contents")
            return None
        
        # Check if dictionaries are the same size
        if d1 == d2:
            print("No difference")
            return None
        
        # Return the larger Dictionary with a Max() comparison
        else:
            decider = max(d1, d2)
            if d1 == decider:
                print(dict1)
                return dict1
            else:
                print(dict2)
                return dict2
```
