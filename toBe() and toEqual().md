### toBe() and toEqual()

**We can use toBe for primitives like strings, numbers or Booleans,  for everything else use toEqual.**

**Example :**

<pre>
import { CUSTOM_ELEMENTS_SCHEMA } from '@angular/core';
import { TestBed } from '@angular/core/testing';

import { RouterTestingModule } from '@angular/router/testing';

import { AppComponent } from './app.component';

describe('AppComponent', () => {


  beforeEach(async () => {

    await TestBed.configureTestingModule({
      declarations: [AppComponent],
      schemas: [CUSTOM_ELEMENTS_SCHEMA],
      imports: [RouterTestingModule.withRoutes([])],
    }).compileComponents();
  });

  it('should create the app', async () => {
    const fixture = TestBed.createComponent(AppComponent);
    const app = fixture.componentInstance;
    expect(app).toBeTruthy();
  });
  it('should return a message',async () => {
    let component = new AppComponent();
    expect(component.returnAmessage('hello')).toBe('hello')
  })

  it('should equal the result', () => {
    const a:number = 5;
    const b:number= 5;

    let name1 = 'Somrat';
   let name2 = 'Somrat';

   let array1 = ['A','B'];
    let array2 = ['A', 'B'];

    let obj1 = {name:'somrat', id: 211015116}
    let obj2 = {name:'somrat', id: 211015116}

    // number comapare using toBe matcher;
    expect(a).toBe(b); // output: true

    // number compare using toEqual matcher;
    expect(a).toEqual(b); // output: true

    // string compare using toBe matcher;
    expect(name1).toBe(name2); // output: true

    // string compare using toEqual matcher;
    expect(name1).toEqual(name2); // output: true

    // array compare using toBe matcher;
    expect(array1).toBe(array2); // output: false

    // array compare using toEqual mathcer;
     expect(array1).toEqual(array2); // output: true

    // object compare using toBe matcher;
     expect(obj1).toBe(obj2); // output: false

    // object compare using toEqual matcher;

    expect(obj1).toEqual(obj2); // output: true



  });



});

</pre>
