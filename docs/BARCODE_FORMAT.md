# Barcode Format Reference

## Format Structure

```
Y YYYYY AABBB X
```

- **Y YYYYY**: Doesn't matter, just normal barcode numbers
- **AA**: Identifier (00-99)
- **BBB**: Sub-identifier (000-999)
- **X**: Normal barcode check digit, does have to be right 

## AA Identifier Ranges

### AA 00-39: Races (63 total configurations)
It might *seem* like you can break down `BBB` into further things but it's really just a sequential list. 

- [Race List](./RACES.md)

### AA 40-99: Cars and Parts

- **BBB 000-399**: Car identification [Car List](./CARS.md)
- **BBB 400-999**: Part identification [Part List](./ITEMS.md)

