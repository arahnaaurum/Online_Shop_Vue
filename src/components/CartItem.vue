<template>
    <div class="cart-item">
        <div class="product-bio">
            <img src="https://i.pinimg.com/736x/23/73/71/2373711bb68a06da91c0ffd3d5235ef8--pink-lady-lady-gaga-pink.jpg" width=50 alt="Clothes">
                <div class="product-desc">
                    <h1 class="product-title pinktext">{{cartItem.product_name}}</h1>
                    <p class="product-quantity">Quantity: {{cartItem.quantity}}</p>
                    <p class="product-single-price">Price: {{cartItem.price}}</p>
                </div>
        </div>
        <div class="right-block">
            <p class="product-price">Total: {{cartItem.quantity*cartItem.price}}</p>
            <button class="del-btn" @click="$emit('remove', cartItem)">&times;</button>
         </div>
    </div>
</template>

<script>
export default {
    name: "CartItem",
    props: ['cartItem'],
};
</script>