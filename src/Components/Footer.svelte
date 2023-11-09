<script>
    import { Link } from "svelte-routing";
    import logoWhite from '/assets/img/logo-white.png';
    import visa from '/assets/img/visa.png';
    import mastercard from '/assets/img/mastercard.png';
    import payoneer from '/assets/img/payoneer.png';
    import paypal from '/assets/img/paypal.png';
</script>

<footer class="footer pt-100">
    <div class="footer-top pb-60">
        <div class="container">
            <div class="row">
                <div class="col-lg-4 col-md-6">
                    <div class="footer-widget footer-widget-1">
                        <Link to="home" class="footer-logo"><img src={logoWhite} class="logo" alt="logo"></Link>
                        <p class="text-white mt-30">My service is not something I even think about because it is always there as we agreed. The customer service is responsive and knowledge needs for</p>
                        <div class="footer-social mt-5">
                            <h5 class="ft-subtitle text-white position-relative d-inline-block">Follow us on</h5>
                            <ul class="social-nav mt-3">
                                <li><Link to="home" class="rounded-circle overflow-hidden position-relative d-flex align-items-center justify-content-center text-white"><i class="fab fa-facebook-f"></i></Link></li>
                                <li><Link to="home" class="rounded-circle overflow-hidden position-relative d-flex align-items-center justify-content-center text-white"><i class="fab fa-twitter"></i></Link></li>
                                <li><Link to="home" class="rounded-circle overflow-hidden position-relative d-flex align-items-center justify-content-center text-white"><i class="fab fa-instagram"></i></Link></li>
                                <li><Link to="home" class="rounded-circle overflow-hidden position-relative d-flex align-items-center justify-content-center text-white"><i class="fab fa-linkedin"></i></Link></li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-lg-2 col-md-3 col-sm-6">
                    <div class="footer-widget footer-widget-2 mt-2">
                        <h5 class="text-white position-relative mb-5 widget-title">Quick Links</h5>
                        <ul class="footer-nav">
                            <li><Link to="contact">Support Center</Link></li>
                            <li><Link to="about">About Us</Link></li>
                            <li><Link to="home">My Account</Link></li>
                        </ul>
                    </div>
                </div>
                <div class="col-lg-2 col-md-3 col-sm-6">
                    <div class="footer-widget footer-widget-3 mt-2">
                        <h5 class="text-white position-relative mb-5 widget-title">Services</h5>
                        <ul class="footer-nav">
                            <li><Link to="shared-hosting">Shared Hosting</Link></li>
                            <li><Link to="vps-hosting">VPS Hosting</Link></li>
                            <li><Link to="dedicated-server">Dedicated Hosting</Link></li>
                        </ul>
                    </div>
                </div>
                <div class="col-lg-4 col-md-8">
                    <div class="footer-widget footer-sb-widget mt-2">
                        <h5 class="text-white position-relative mb-5 widget-title">Get In Touch</h5>
                        <form action="#" class="footer-sb-form position-relative">
                            <input type="email" placeholder="Type Your Mail">
                            <button type="submit" class="template-btn primary-btn btn-small">Subscribe</button>
                        </form>
                        <div class="ft-payment-method mt-40">
                            <h5 class="text-white position-relative ft-subtitle d-inline-block">We Accepted</h5>
                            <ul class="payment-list d-flex align-items-center mt-3">
                                <li class="d-inline-flex align-items-center justify-content-center"><img src={visa} alt="visa" class="img-fluid"></li>
                                <li class="d-inline-flex align-items-center justify-content-center"><img src={mastercard} alt="mastercard" class="img-fluid"></li>
                                <li class="d-inline-flex align-items-center justify-content-center"><img src={payoneer} alt="payoneer" class="img-fluid"></li>
                                <li class="d-inline-flex align-items-center justify-content-center"><img src={paypal} alt="paypal" class="img-fluid"></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="footer-copyright">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-md-6">
                    <div class="copyright-txt text-white">
                        <p class="mb-0">Copyright 2022 Hostim. All Rights Reserved</p>
                    </div>
                </div>
                <div class="col-md-6">
                    <div class="copyright-links mt-2 mt-md-0 text-start text-md-end">
                        <Link to="home">Terms & Conditions</Link>
                        <Link to="home" class="ml-20">Privacy Policy</Link>
                    </div>
                </div>
            </div>
        </div>
    </div>
</footer>