document.addEventListener("DOMContentLoaded", function() {
    const products = [
        {
            name: "Apple",
            price: "$1.00 each",
            image: "apple.jpg"
        },
        {
            name: "Banana",
            price: "$0.50 each",
            image: "banana.jpg"
        },
        {
            name: "Carrot",
            price: "$0.30 each",
            image: "carrot.jpg"
        },
        {
            name: "Broccoli",
            price: "$1.50 each",
            image: "broccoli.jpg"
        },
        {
            name: "Tomato",
            price: "$0.70 each",
            image: "tomato.jpg"
        },
        {
            name: "Orange",
            price: "$0.80 each",
            image: "orange.jpg"
        },
        {
            name: "Potato",
            price: "$0.40 each",
            image: "potato.jpg"
        },
        {
            name: "Strawberry",
            price: "$2.00 per pack",
            image: "strawberry.jpg"
        },
        {
            name: "Grapes",
            price: "$3.00 per bunch",
            image: "grapes.jpg"
        }
    ];

    const productList = document.getElementById("product-list");

    products.forEach(product => {
        const productCard = `
            <div class="col-md-4 col-sm-6 mb-4">
                <div class="card">
                    <img src="${product.image}" class="card-img-top" alt="${product.name}">
                    <div class="card-body">
                        <h5 class="card-title">${product.name}</h5>
                        <p class="card-text">${product.price}</p>
                        <a href="#" class="btn btn-primary">Add to Cart</a>
                    </div>
                </div>
            </div>
        `;
        productList.innerHTML += productCard;
    });
});
