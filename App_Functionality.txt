import React, { Component } from 'react';
import { AppRegistry, Text, View, StyleSheet, Image, TextInput, ImageBackground, TouchableHighlight, Alert, Dimensions, ScrollView } from 'react-native';
import Constants from 'expo-constants';

let deviceHeight = Dimensions.get('window').height;
let deviceWidth = Dimensions.get('window').width;


export default class App extends Component {
    state ={
        zodiac:'Zodiac',
        zodiacImage: 'https://codehs.com/uploads/a378f86890cf1439087cfd6974acc83f',
        description: 'Enter your month (left box) and day (right box) of birth below',
        month: '',
        day: '',
    }
    updateZodiac =()=> {
        if ((this.state.month == 1 && (this.state.day > 20 && this.state.day < 32)) || (this.state.month == 2 && (this.state.day < 19 && this.state.day > 0))){
            
        this.setState({
            zodiac: 'Aquarius',
            zodiacImage: 'https://codehs.com/uploads/f317449eec3b36313599e9d923494f25',
            description: 'Aquarius people are advanced, self-reliant, clever, exceptional, and optimistic. Air is their elemental sign. Aquarians, like air, lack a distinct form and appear to resist classification. Others are enthusiastic and active, while other Aquarians are calm and sensitive.',
        })
        }
        else if ((this.state.month == 2 && (this.state.day > 18 && this.state.day < 30)) || (this.state.month == 3 && (this.state.day < 21 && this.state.day > 0))){
            
        this.setState({
            zodiac: 'Pisces',
            zodiacImage: 'https://codehs.com/uploads/63208c3e1ec5a9a8cb6f06395a4b27dc',
            description: 'Pisces is a sensitive water sign, ruled by the planet Neptune. Your sign is fluid and tends to be sympathetic to the underdog. Its so easy for you to feel other peoples experiences that they can obscure your own. You can be vague and escapist, but make up for it by being compassionate and intuitive.',
        })
        }
        else if ((this.state.month == 3 && (this.state.day > 20 && this.state.day < 32)) || (this.state.month == 4 && (this.state.day < 20 && this.state.day > 0))){
            
        this.setState({
            zodiac: 'Aries',
            zodiacImage: 'https://codehs.com/uploads/0a99b2e4afc807c0525e07a81ac9256a',
            description: 'Aries are spontaneous and courageous. They have a sense of adventure and love to explore. Theyre determined and bold, and are good at initiating new projects. They have high energy and can initiate quick actions.',
        })
        }
         else if ((this.state.month == 4 && (this.state.day > 19 && this.state.day < 31)) || (this.state.month == 5 && (this.state.day < 21 && this.state.day > 0))){
            
        this.setState({
            zodiac: 'Taurus',
            zodiacImage: 'https://codehs.com/uploads/84c3f6379d4388591fb18bf1d886e41d',
            description: 'Taurus natives like the Bull who represents their sign, are prone to anger, but once enraged, they can be terrifying. People born under the Taurus sign appreciate integrity above all else.',
        })
        }
        else if ((this.state.month == 5 && (this.state.day > 20 && this.state.day < 32)) || (this.state.month == 6 && (this.state.day < 21 && this.state.day > 0))){
            
        this.setState({
            zodiac: 'Gemini',
            zodiacImage: 'https://codehs.com/uploads/ec6600b706864882ef3ba420fe867c7e',
            description: 'Geminis are volatile beings that are inquisitive, intelligent, and great thinkers. They tend to remain in one location. ... The Gemini personality is a lot of fun, but it does have flaws, just like any other sign. Geminis are flexible, extroverted, and clever, and theres never a boring moment while theyre around.',
        })
        }
        else if ((this.state.month == 6 && (this.state.day > 20 && this.state.day < 31)) || (this.state.month == 7 && (this.state.day < 23 && this.state.day > 0))){
            
        this.setState({
            zodiac: 'Cancer',
            zodiacImage: 'https://codehs.com/uploads/c4f513364aa5205b89900b903aac1330',
            description: 'Cancers have a reputation for being hyper emotional, temperamental, and spiteful. Cancers, in additional to being devoted, are extremely fond of their loved ones, often to an unhealthy degree. They place a high value on family and close friends, and will go to great lengths to defend them, no matter the price.',
        })
        }
        else if ((this.state.month == 7 && (this.state.day > 22 && this.state.day < 32)) || (this.state.month == 8 && (this.state.day < 23 && this.state.day > 0))){
            
        this.setState({
            zodiac: 'Leo',
            zodiacImage: 'https://codehs.com/uploads/58bb234b107511b84ce48919e9ce38e4',
            description: 'Leos are the natural leaders of the zodiac, as magnificent and striking as the Lion that embodies their sign. Leos are radiantly joyful, liberal with their appeal and endowments. They are fiercely proud and confident.',
        })
        }
        else if ((this.state.month == 8 && (this.state.day > 22 && this.state.day < 32)) || (this.state.month == 9 && (this.state.day < 23 && this.state.day > 0))){
            
        this.setState({
            zodiac: 'Virgo',
            zodiacImage: 'https://codehs.com/uploads/6949311e3d4e36790099274cb6874f0f',
            description: 'Virgos are logical, practical, and systematic in their approach to life. This earth sign is a perfectionist at heart and isnt afraid to improve skills through diligent and consistent practice.',
        })
        }
        else if ((this.state.month == 9 && (this.state.day > 22 && this.state.day < 31)) || (this.state.month == 10 && (this.state.day < 23 && this.state.day > 0))){
            
        this.setState({
            zodiac: 'Libra',
            zodiacImage: 'https://codehs.com/uploads/8e3ebb7d20b8cb066135407b37cb3363',
            description: 'Libras are extroverted, cosy, and friendly people. Librans, like the Scales that symbolise the sign, are often concerned with attaining balance, harmony, peace, and justice in the world.',
        })
        }
        else if ((this.state.month == 10 && (this.state.day > 22 && this.state.day < 32)) || (this.state.month == 11 && (this.state.day < 22 && this.state.day > 0))){
            
        this.setState({
            zodiac: 'Scorpio',
            zodiacImage: 'https://codehs.com/uploads/1db518c03f7f622ab1e22ed2086b6e0e',
            description: 'The Scorpio personality is often misunderstood due to their intensity and their tendency to be harsh. However, Scorpios are extremely emotional, and crave intimacy. They have a powerful presence and demanding personalities, and their penchant for mystery is what makes them one of the most interesting signs.',
        })
        }
        else if ((this.state.month == 11 && (this.state.day > 21 && this.state.day < 32)) || (this.state.month == 12 && (this.state.day < 22 && this.state.day > 0))){
            
        this.setState({
            zodiac: 'Sagitarius',
            zodiacImage: 'https://codehs.com/uploads/eafe3c8d4cb421f3d78bd86de431c15f',
            description: 'Sagittarius natives are loyal, smart, assertive, and compassionate personality! They are one-of-a-kind, talented, and have impeccable discernment. They are a fantastic, caring personality type because of their blend of autonomy, intellect, and empathy.',
        })
        }
         else if ((this.state.month == 12 && (this.state.day > 21 && this.state.day < 32)) || (this.state.month == 1 && (this.state.day < 21 && this.state.day > 0))){
            
        this.setState({
            zodiac: 'Capricorn',
            zodiacImage: 'https://codehs.com/uploads/11318d2409982a0082d7ec37f3ba8e4c',
            description: 'Capricorns are the ultimate worker bees; theyre ambitious, organized, practical, goal-oriented, and they dont mind the hustle. “Theyre ready to give up a lot in order to achieve that goal,” Verk says. They also love making their own rules, which means they strive to reach high career positions.',
        })
        }
        else{
            this.setState ({
            zodiac:'Error',
            zodiacImage: 'https://codehs.com/uploads/a378f86890cf1439087cfd6974acc83f',
            description: 'Unrecgonized Input. Please try again, make sure to use numbers for the month instead of typing the month name.',
            })
        }
    }
    
    dayChange = day =>{
        this.setState({day})
    }
    monthChange = month =>{
        this.setState({month})
    }
    
    render() {
        return (
            <View style={styles.container}>
                <ImageBackground
                style={styles.background}
                source= {{uri: 'https://codehs.com/uploads/a378f86890cf1439087cfd6974acc83f'}}
                >
                    <View style={styles.container}>
                        <View style={styles.zodiacContainer}>
                            <Text style={styles.largeText}>
                                {this.state.zodiac}
                            </Text>
                            <Image
                            source ={{uri: this.state.zodiacImage}}
                            style ={styles.zodiac}
                            />
                            <View style={styles.informationContainer}>
                                <Text style={styles.information}>
                                {this.state.description}
                                </Text>
                            </View>
                        </View>
                        <View style={styles.inputContainer}>
                            <View style={styles.textRow}>
                                <View style={styles.inputBox}>
                                    <TextInput
                                    value = {this.state.month}
                                    onChangeText ={this.monthChange}
                                    style = {styles.buttonText}
                                    />
                                </View>
                                <View style={styles.inputBox}>
                                     <TextInput
                                    value = {this.state.day}
                                    onChangeText ={this.dayChange}
                                    style = {styles.buttonText}
                                    />
                                
                                </View>
                            </View>
                            <TouchableHighlight
                            style = {styles.button}
                            onPress= {this.updateZodiac}
                            >
                                <Text style ={styles.buttonText}>
                                ZODIAC!
                                </Text>
                            </TouchableHighlight>
                        </View>
                    </View>
                </ImageBackground>
            </View>
        );
    }
}

const styles = StyleSheet.create({
    container: {
        height: deviceHeight,
        width: deviceWidth,
    },
     background: {
     
        justifyContent: 'center',
        alignItems: 'center',
    },
    zodiacContainer:
    {
        height: 4*(deviceHeight/5),
        justifyContent: 'center',
        alignItems: 'center',
    },
    inputContainer:
    {
        height: deviceHeight/5,
        justifyContent: 'center',
        alignItems: 'center',

    },
    largeText:
    {
        color: '#bc81e3',
        fontSize: 50,
        fontWeight: 'bold',
    },
    zodiac:
    {
        height: 175,
        width: 175,
        margin: 20,
    },
    informationContainer:
    {
        width: deviceWidth/1.2
    },
    information:
    {
        color: '#bc81e3',
        fontSize: 15,
        textAlign: 'left',
    },
    textRow:
    {
        flexDirection: 'row',
        justifyContent: 'center',
        alignItems: 'center',
    },
    inputBox:
    {
        height: deviceHeight/12,
        width: deviceWidth/3,
        backgroundColor: '#bc81e3',
        borderColor: 'purple',
        borderWidth: 3,
        margin: 5,
        justifyContent: 'center',
    },
    button:
    {
        height: deviceHeight/10,
        width: deviceWidth/2.5,
        backgroundColor: 'purple',
        borderColor: '#bc81e3',
        borderWidth: 2,
        justifyContent: 'center',
        alignItems: 'center',
    },
    buttonText:
    {
        fontWeight: 'bold',
    },
});