1. Create a basic html file

2. Creat class and extends the HTMLElements

3. we will create a constructor

4. we need to define The Element

5. Then here going to pass some properties

   # this.innerHTML = `<h3>${this.getAttribute('name')}</h3>`;

6. Lets Add some style

   # this.innerHTML = `<style>h3{color: blue;}</style><h3>${this.getAttribute('name')}</h3>`;

7. Then we are going to encapsulate every thing into webcomponents

8. To do that we are going to attach shadowDOM

   # this.attachShadow({mode:'open'})

9. Then we are going to use shadowRoot and append template

   # this.shadowRoot.appendChild(template.content.cloneNode(true));

10. Now we are going to create template
    # const template = document.createElement('template');
    # template.innerHTML = `<style>h3{color: blue;}</style><div class="user-card"><h3></h3></div>`;
    # this.shadowRoot.querySelector('h3').innerText = this.getAttribute('name');
    # add some Avatar https://randomuser.me/api/portraits/women/1.jpg
    # this.shadowRoot.querySelector('img').src = this.getAttribute('avatar');

11. Then we are going to use slots to bring up the values
    <!--<user-card name="Jane Doe" avatar="https://randomuser.me/api/portraits/women/1.jpg">
        <div slot="email">janedoe@gmail.com</div>
        <div slot="phone">333-333-3333</div>
    </user-card> -->

12. Put some Eventlistner in lifecycle methods 
    # connectedCallback() {  }
    # disconnectedCallback() {  } 



