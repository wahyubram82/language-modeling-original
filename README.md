# Language Modeling

This is machine learning model that is trained to predict next word in the sequence.
Model is defined in keras and then converted to tensorflowjs model using tfjs_converter.


## [See it working!](https://nxt-word.firebaseapp.com)

## Dependencies

* [keras](https://github.com/keras-team/keras)
* [tensorflow](https://www.tensorflow.org/)
* [tensorflowjs_converter](https://js.tensorflow.org/) (for web deployment)

To install all dependencies at once use:

```
pip3 install -r requirements.txt
```

## Usage

Once you have your dependencies installed via pip, train the model by running

```
python3 train.py
```
After training you can either use the model by running

```
python3 test.py
```
or by converting the model to tensorflow js model by running
```
tensorflowjs_converter --input_format=keras /mode/model.h5 /web/web_model
```
then serve the /web directory to a local server.


## [License MIT © Rajveer Malviya](https://github.com/rajveermalviya/language-modeling/blob/master/LICENSE.md)