# API de Produtos
#### API de produtos criada para o Hackathon da Laboratoria :)

A API de produtos pode ser consumida através da URL: http://my-json-server.typicode.com/jusbrasil/hackathon-laboratoria e o formato de retorno é o JSON.

## Endpoints
Você pode obter a listagem e os detalhes dos produtos através de dois endpoints:

### 1) Listagem de produtos
**Endpoint:** `/product-list`

**Exemplo de retorno**
```bash
$ curl http://my-json-server.typicode.com/jusbrasil/hackathon-laboratoria/product-list

[
    {
      "id": 100,
      "name": "Product Name",
      "price": 1000,
      "thumbnail": "https://www.domain.com/image-path.png"
    },
    {
      "id": 200,
      "name": "Another product",
      "price": 2000,
      "thumbnail": "https://www.domain.com/another-image-path.png"
    }
]

```

#### 2) Detalhes do produto
**Endpoint:** `/products/$PRODUCT_ID`

**Exemplo de retorno**
```bash
{
  "name": "Product Name",
  "description": "Description of the product",
  "price": 1000.0,
  "stock_amount": 10,
  "image": "https://www.domain.com/path-of-image.png"
}
```
