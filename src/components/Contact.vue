<template>
    <div class="contact-container" id="contact">
        <div class="title">
            <h2>contact</h2>
            <h1>get in touch</h1>
        </div>
        <div class="content">
            <div class="card">
                <h1>Phone</h1>
                <p>+961 81 830 544</p>
            </div>
            <div class="card">
                <h1>Email</h1>
                <p>letsmailali@gmail.com</p>
            </div>
            <div class="card">
                <h1>Address</h1>
                <p>Lebanon, Beirut, Mar Elias</p>
            </div>
        </div>
        <div class="form-container">
            <form target="_blank" action="https://formsubmit.co/5f586025505f1fa25556f1a2b8b79b4f" method="POST">
                <div class="form-group">
                    <input type="text" name="name" placeholder="Name" required>
                    <input type="email" name="email" placeholder="Email">
                    <input type="text" name="subject" placeholder="Subject" required>
                </div>
                <div class="form-group">
                    <textarea name="message" rows="10" placeholder="Message" required></textarea>
                    <button type="submit"><span>Send Message</span></button>
                </div>
            </form>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Contact',

    }
</script>

<style scoped>
    .contact-container{
        position: relative;
        width: 100%;
        margin: 15rem 0;
    }
    .contact-container .title{
        width: 100%;
        position: relative;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-bottom: 10rem;
    }
    .contact-container .title h2{
        font-size: 3rem;
        color: var(--accent-1);
        text-transform: uppercase;
    }
    .contact-container .title h1{
        font-size: 5rem;
        color: var(--accent-2);
        text-transform: uppercase;
    }
    .contact-container .content{
        position: relative;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
    }
    .contact-container .content .card{
        position: relative;
        width: 50rem;
        /* height: 10rem; */
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
        padding: 2rem;
        border-top: 2px solid var(--accent-2);
        border-left: 2px solid var(--accent-2);
        border-bottom: 2px solid var(--accent-1);
        border-right: 2px solid var(--accent-1);
        border-radius: 2rem;
        margin: 2rem;
    }
    .contact-container .content .card h1{
        font-size: 2.5rem;
        color: var(--accent-2);
        text-transform: uppercase;
    }
    .contact-container .content .card p{
        font-size: 1.5rem;
        color: var(--font-light);
        margin: 1rem;
    }
    .form-container{
        position: relative;
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin: 10rem 0;
    }
    .form-container form{
        position: relative;
        padding: 2rem;
        border-radius: 2rem;
        border: 2px solid var(--accent-1);
        display: flex;
    }
    .form-container form .form-group{
        position: relative;
        display: flex;
        flex-direction: column;
        align-items: flex-end;

    }
    .form-container form .form-group input{
        width: 40rem;
        padding: 1rem 2rem;
        border-radius: 2rem;
        background: none;
        border: 2px solid var(--accent-1);
        outline: none;
        margin: 1rem;
        color: var(--font-light);
    }
    .form-container form .form-group input:focus{
        border: 2px solid var(--accent-2);
    }
    .form-container form .form-group input::placeholder{
        font-size: 1.5rem;
        color: var(--accent-1);
    }
    .form-container form .form-group textarea{
        padding: 1rem 2rem;
        border: 2px solid var(--accent-1);
        margin: 1rem;
        width: 60rem;
        height: 30rem;
        background: none;
        color: var(--font-light);
        outline: none;
    }
    .form-container form .form-group textarea::-webkit-scrollbar {
        width: 1rem;
        padding: 2rem;
    }   
 
    .form-container form .form-group textarea::-webkit-scrollbar-track {
        background: var(--accent-1);
        border-radius: 3rem;
    }
    
    .form-container form .form-group textarea::-webkit-scrollbar-thumb {
        background-color: var(--accent-2);
        border-radius: 3rem;
    }
    .form-container form .form-group textarea::placeholder{
        font-size: 1.5rem;
        color: var(--accent-1);
    }
    .form-container form .form-group textarea:focus{
        border: 2px solid var(--accent-2);
    }
    .form-container form button{
        background: none;
        border: none;
        margin: 2rem;
        margin-right: 0;
    }
    .form-container form button:hover{
        cursor: pointer;
    }
    .form-container form button span{
        padding: .5rem 1rem;
        /* background: var(--accent-2); */
        border-radius: 2rem;
        border: 2px solid var(--accent-2);
        color: var(--font-light);
        font-size: 1.5rem;
    }
    .form-container form button:hover span{
        background: var(--accent-2);
    }
    @media screen and (max-width: 1200px) {
        .contact-container{
            margin: 5rem 0;
            width: 100%;
            padding: 0 2rem;
        }
        .contact-container .title h2{
            font-size: 1.5rem;
        }
        .contact-container .title h1{
            font-size: 3rem;
        }
        .contact-container .title{
            margin-bottom: 5rem;
        }
        .form-container{
            margin-top: 3rem;
        }
        .form-container form{
            width: 100%;
        }
        .form-container form .form-group:nth-child(1){
            width: 30%;
        }
        .form-container form .form-group:nth-child(2){
            width: 70%;
        }
        .form-container form .form-group input{
            width: 100%;
            margin: 1rem;
        }
        .form-container form .form-group textarea{
            width: unset;
            height: unset;
            margin: 0;
            width: 100%;
        }
        
    }
    @media screen and (max-width: 992px) {
        .contact-container{
            margin: 5rem 0;
            width: 100%;
            padding: 0 2rem;
        }
        .contact-container .title h2{
            font-size: 1.5rem;
        }
        .contact-container .title h1{
            font-size: 3rem;
        }
        .contact-container .title{
            margin-bottom: 5rem;
        }
        .form-container{
            margin-top: 3rem;
        }
        .form-container form{
            flex-direction: column;
            width: 100%;
        }
        .form-container form .form-group:nth-child(1){
            width: 100%;
        }
        .form-container form .form-group:nth-child(2){
            width: 100%;
        }
        .form-container form .form-group input{
            width: 100%;
            margin: 1rem;
        }
        .form-container form .form-group textarea{
            width: unset;
            height: unset;
            margin: 0;
            width: 100%;
        }
        
    }
    @media screen and (max-width: 768px) {
        .contact-container{
            margin: 5rem 0;
            width: 100%;
            padding: 0 2rem;
        }
        .contact-container .title h2{
            font-size: 1.5rem;
        }
        .contact-container .title h1{
            font-size: 3rem;
        }
        .contact-container .title{
            margin-bottom: 5rem;
        }
        .form-container{
            margin-top: 3rem;
        }
        .form-container form{
            flex-direction: column;
            width: 100%;
        }
        .form-container form .form-group:nth-child(1){
            width: 100%;
        }
        .form-container form .form-group:nth-child(2){
            width: 100%;
        }
        .form-container form .form-group input{
            width: 100%;
            margin: 1rem;
        }
        .form-container form .form-group textarea{
            width: unset;
            height: unset;
            margin: 0;
            width: 100%;
        }
        
    }
    @media screen and (max-width: 576px) {
        .contact-container{
            margin: 5rem 0;
            width: 100%;
            padding: 0 2rem;
        }
        .contact-container .title h2{
            font-size: 1.5rem;
        }
        .contact-container .title h1{
            font-size: 3rem;
        }
        .contact-container .title{
            margin-bottom: 5rem;
        }
        .form-container{
            margin-top: 3rem;
        }
        .form-container form{
            flex-direction: column;
            width: 100%;
        }
        .form-container form .form-group:nth-child(1){
            width: 100%;
        }
        .form-container form .form-group:nth-child(2){
            width: 100%;
        }
        .form-container form .form-group input{
            width: 100%;
            margin: 1rem;
        }
        .form-container form .form-group textarea{
            height: unset;
            margin: 0;
            width: 100%;
        }
        
    }
</style>